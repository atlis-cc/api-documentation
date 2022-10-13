Data Transfer Objects (DTO)
===========================
Data Transfer Objects determine how incoming data should look per-route.

* Optional, not required
* Recommended for readability and type safety

DTO Template
------------
<> = replace

.. code-block:: typescript
    :name: dto_example
    
    export interface <Action><Resource>Dto {
        <inputName>: <inputType>;
    }

| **<Action>** The type of action of the route (Get, Create, Update, Delete, etc.)
| **<Resource>** The resource being accessed (User, Post, etc.)
| **<inputName>** The field in the request body
| **<inputType>** The JavaScript type of data (string, boolean, number[], etc.)
