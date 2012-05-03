A basic `Admin` for a Propel model is defined by this service:

```yaml
services:
    depot.admin:
        class: Ormigo\Bundle\TransactionBundle\Admin\DepotAdmin
        arguments:
            - ~
            - 'Ormigo\Bundle\TransactionBundle\Model\Depot'
            - ''
        tags:
            -
                name: 'sonata.admin'
                manager_type: 'propel'
                group: 'Transactions'
                label: 'Depot'
```