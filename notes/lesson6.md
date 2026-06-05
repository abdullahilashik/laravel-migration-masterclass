migrate
  -> Runs only pending migrations
  -> Never touches what is already applied
  -> Safe for production
  -> Data is preserved

migrate:refresh
  -> Rolls back all migrations using down() methods
  -> Then re-runs everything from scratch
  -> Requires correct down() methods to work
  -> All data is destroyed
  -> Local development only

migrate:fresh
  -> Drops every table in the database directly
  -> Ignores down() methods completely
  -> Works even with broken or missing down() methods
  -> All data is destroyed
  -> Local development only