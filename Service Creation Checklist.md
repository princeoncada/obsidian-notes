- [ ] Create EntityDTO and define 2 or 3 data classes; 
	-  1 for get result, 
	-  1 for post request, and 
	-  1 for put request.

- [ ] Create EntityMapper

- [ ] Create EntityService;

- [ ] Include in EntityRepository 
	- findById(id: String, pageable: Pageable): Page<\Entity>

- [ ] Create EntityServiceImpl
- [ ] Create EntityController


_______________________________________________________

- [ ] Create EntityDTO and define 2 or 3 data classes; 
	- 1 for get request, 
	- 1 for post request, and 
	- 1 for optional put request.



- [ ] Create EntityService and define 5 functions;
	- 1 for getEntities(
			pageable: Pageable
		): Page<EntityDTOs.EntityDTO>
		
	- 1 for getEntityById(
			id: String, 
			pageable: Pageable
		): Page<EntityDTOs.EntityDTO>
		
	- 1 for createEntity(
			entityRequest: EntityDTOs.postRequest, 
			pageable: Pageable
		): Page<EntityDTOs.EntityDTO>
		
	- 1 for updateEntityById(
			id: String, 
			entityRequest: EntityDTOs.putRequest
			pageable: Pageable
		): Page<EntityDTOs.EntityDTO>
		
	- 1 for deleteEntitybyId(
			id: String, 
			pageable: Pageable
		): Page<EntityDTOs.EntityDTO>


- [ ] Include in EntityRepository 
	- findById(id: String, pageable: Pageable): Page<\Entity>


- [ ] Create EntityServiceImpl
- [ ] Create EntityController
