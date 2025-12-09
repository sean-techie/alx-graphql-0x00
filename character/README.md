# GraphQL Query
The GraphQL query is defined in character-id-1.graphql

query character($id: ID!) {
    character(id: $id) {
            id
                    name
                            status
                                    species
                                            type
                                                    gender
                                                        }
                                                        }
                                                        Response
                                                        The response is defined in character-id-1-output.json.

                                                        {
                                                            "data": {
                                                                    "character": {
                                                                                "id": "1",
                                                                                            "name": "Rick Sanchez",
                                                                                                        "status": "Alive",
                                                                                                                    "species": "Human",
                                                                                                                                "type": "",
                                                                                                                                            "gender": "Male"
                                                                                                                                                    }
                                                                                                                                                        }
                                                                                                                                                        }
                                                                                                                                                        