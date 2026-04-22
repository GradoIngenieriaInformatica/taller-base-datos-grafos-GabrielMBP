MATCH (p:Persona)-[:ESTUDIO_EN]->(u:Universidad) 
WITH u, count(p) as num_estudiantes 
WHERE num_estudiantes > 1 
RETURN u.nombre