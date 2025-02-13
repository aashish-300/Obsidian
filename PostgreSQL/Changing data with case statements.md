
SELECT
  staff_name,
  weight_kg,
  CASE
    WHEN weight_kg < 10 then weight_kg * 10
    ELSE weight_kg
  end as fixed_weight
from
  crew
  where weight_kg < 10
order by
  fixed_weight asc;