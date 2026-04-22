MATCH (p:Persona)-[:AMIGO_DE]-(amigo:Persona)-[:PARTICIPA_EN]->(pr:Proyecto) WHERE NOT (p)-[:PARTICIPA_EN]->(pr) RETURN DISTINCT p.nombre AS Persona;
