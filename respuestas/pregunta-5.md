MATCH (p1:Persona)-[:VIVE_EN]->(c:Ciudad)<-[:VIVE_EN]-(p2:Persona), (p1)-[:TRABAJA_CON]-(p2)
WHERE id(p1) < id(p2)
RETURN p1.nombre, p2.nombre>