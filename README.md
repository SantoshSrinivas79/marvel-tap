# marvel_tap

This is an unofficial [Singer](https://singer.io) tap that produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md).

This tap:
- Pulls raw data from Marvel's [REST API](https://developer.marvel.com/)
- Extracts the following resources from Marvel:
  - [Characters](https://developer.marvel.com/docs#!/public/getCreatorCollection_get_0)
- Outputs the schema for each resource
- Incrementally pulls data based on the input state
- Dumps everything into a CSV called characters

