# reactivities-sw4-master
Trabajo Final 


       public Handler(DataContext context){
                _context = context;
            }
            public async Task<Activity> Handle(QueryId request, CancellationToken cancellationToken){
                return await _context.Activities.FindAsync(request._guid);
            }
