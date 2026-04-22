MATCH (p:Persona)-[:USA_TECNOLOGIA]->(t:Tecnologia {nombre:"Python"}), (p)-[:TRABAJA_EN]->(e:Empresa) 
RETURN DISTINCT e.nombre