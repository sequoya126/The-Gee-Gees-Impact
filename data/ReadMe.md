# Organization Data Schema

| Column | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| id | string | Yes | Unique slug (e.g., "ottawa-food-bank") |
| name | string | Yes | Organization name |
| category | string | Yes | e.g., "Food Security", "Youth" |
| neighbourhood | string | Yes | Must match a `NAME` in the GeoJSON |
| address | string | No | Street address |
| website | string | No | URL |
| contact_email | string | No | Public contact email |
| description | string | No | 1–2 sentence summary |