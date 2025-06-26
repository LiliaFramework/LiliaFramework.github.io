        ## Provides compatibility with the DarkRP gamemode.

        **Description:**
            Maps functions such as entity creation, money formatting and
empty position checks so DarkRP addons work with the Lilia framework.

        ---

        ### Parameters

            None

        ---

        ### Returns

            None

        ---

        ### Example

            ```lua
            ```

        ## lia.darkrp.isEmpty(position, entitiesToIgnore)

        **Description:**
            Checks whether the specified position is free from players, NPCs,
and props.

        ---

        ### Parameters

            * **position** *(Vector)*: World position to test.
            * **entitiesToIgnore** *(table)*: Entities ignored during the check.

        ---

        ### Returns

            * boolean – True if the position is clear, false otherwise.

        ---

        **Realm:**
            Server

        ---

        ### Example

            ```lua
            if lia.darkrp.isEmpty(Vector(0,0,0)) then
            print("Spawn point is clear")
            end
            ```

        ## lia.darkrp.findEmptyPos(startPos, entitiesToIgnore, maxDistance, searchStep, checkArea)

        **Description:**
            Finds a nearby position that is unobstructed by players or props.

        ---

        ### Parameters

            * **startPos** *(Vector)*: The initial position to search from.
            * **entitiesToIgnore** *(table)*: Entities ignored during the search.
            * **maxDistance** *(number)*: Maximum distance to search in units.
            * **searchStep** *(number)*: Step increment when expanding the search radius.
            * **checkArea** *(Vector)*: Additional offset tested for clearance.

        ---

        ### Returns

            * Vector – A position considered safe for spawning.

        ---

        **Realm:**
            Server

        ---

        ### Example

            ```lua
            local pos = lia.darkrp.findEmptyPos(Vector(0,0,0), nil, 128, 16, Vector(0,0,32))
            ```

        ## lia.darkrp.notify(client, _, _, message)

        **Description:**
            Forwards a notification message to the given client using
lia's notify system.

        ---

        ### Parameters

            * **client** *(Player)*: The player to receive the message.
            * _ – Unused parameter maintained for compatibility.
            * _ – Unused parameter maintained for compatibility.
            * **message** *(string)*: Text of the notification.

        ---

        ### Returns

            * None

        ---

        **Realm:**
            Server

        ---

        ### Example

            ```lua
            lia.darkrp.notify(player.GetAll()[1], nil, nil, "Hello!")
            ```

        ## lia.darkrp.textWrap(text, fontName, maxLineWidth)

        **Description:**
            Wraps a text string so that it fits within the specified width
when drawn with the given font.

        ---

        ### Parameters

            * **text** *(string)*: The text to wrap.
            * **fontName** *(string)*: The font used to measure width.
            * **maxLineWidth** *(number)*: Maximum pixel width before wrapping occurs.

        ---

        ### Returns

            * string – The wrapped text with newline characters inserted.

        ---

        **Realm:**
            Client

        ---

        ### Example

            ```lua
            local wrapped = lia.darkrp.textWrap("Some very long text", "DermaDefault", 150)
            ```

        ## lia.darkrp.formatMoney(amount)

        **Description:**
            Converts a numeric amount to a formatted currency string.

        ---

        ### Parameters

            * **amount** *(number)*: The value of money to format.

        ---

        ### Returns

            * string – The formatted currency value.

        ---

        **Realm:**
            Shared

        ---

        ### Example

            ```lua
            print(lia.darkrp.formatMoney(2500))
            ```

        ## lia.darkrp.createEntity(name, data)

        **Description:**
            Registers a new DarkRP entity as an item so that it can be spawned
through lia's item system.

        ---

        ### Parameters

            * **name** *(string)*: Display name of the entity.
            * **data** *(table)*: Table containing entity definition fields such as
            * model, description, and price.

        ---

        ### Returns

            * None

        ---

        **Realm:**
            Shared

        ---

        ### Example

            ```lua
            lia.darkrp.createEntity("Fuel", {model = "models/props_c17/oildrum001.mdl", price = 50})
            ```

        ## lia.darkrp.createCategory()

        **Description:**
            Placeholder for DarkRP category creation. Currently unused.

        ---

        ### Parameters

            * None

        ---

        ### Returns

            * None

        ---

        **Realm:**
            Shared

        ---

        ### Example

            ```lua
            lia.darkrp.createCategory()
            ```

