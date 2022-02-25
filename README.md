# ADQL code, its just to save my script ;) 

SELECT 
 
  p.ra,p.dec, p.l, p.b, s.z as redshift

FROM PhotoObj AS p

  JOIN SpecObj AS s ON s.bestobjid = p.objid

WHERE 
  
   s.z BETWEEN 0.05 AND 0.075
  
   AND p.ra BETWEEN 150 AND 200
  
   AND p.dec BETWEEN 10 AND 40
