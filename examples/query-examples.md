Query syntax may sometimes be quite obscure, so here are some examples that work


# Querying rollup propery:

`
r = notion.databases.query(
        **{
            "database_id": DB_ID,
            "filter": {"property": "rollupName", 
                        'rollup': {'any': {'text': {'equals': 'value'}}}
            }
        }
        ).get("results")
 `
