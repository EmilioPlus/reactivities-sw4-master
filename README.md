# reactivities-sw4-master
Trabajo Final 


        [HttpGet("{Id}")]
        public async Task<ActionResult<Activity>> GetActivity(Guid Id){
            return Ok();
            retunr await _mediator.Send(new ListById(Id));
        }
    }
}
