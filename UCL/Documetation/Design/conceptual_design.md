# Conceptual Design

#### Entities Based On Initial Study

    - User : User data: includes administration, faculty, and students

    - LAB_ASSISTANT : Lab assistant data: includes graduate assistants

    - WORK_SCHEDULE : Lab assistant work schedule data: hours each lab assistant is assigned to work

    - HOURS_WORKED : Lab assistant hours worked data: actual hours worked per each pay period for each lab assistant

    - LOG : Daily users of the UCL: one entry for each visitor

    - RESERVATION : Lab reservation details

    - INV_TYPE : Inventory types

    - ITEM : Item details

    - LOCATION : Storage locations

    - REPAIR : Repair data by item

    - VENDOR : Vendor details

    - ORDER : Order details

#### Business Rules And Conceptual Model Fragments

Business Rule 1 Each item belongs to only one inventory type, and each inventory type
may have zero, one, or many items belonging to it.

![](./inventory_item_erd.png)

Business Rule 2 An item may be put in use upon its arrival, or it may be stored.

![](./item_storage_location.png)
