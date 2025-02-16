select tc.name from tbl_routine tr

join tbl_group_routine tgr on tr.id = tgr.routine_entity_id

join tbl_group tg on tg.id = tgr.group_entity_id

join tbl_course tc on tc.id = tg.course_entity_id

where tr.id = 11207;