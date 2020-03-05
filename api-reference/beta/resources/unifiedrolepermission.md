---
title: Тип ресурса Унифиедролепермиссион
description: Разрешение роли каталога — это коллекция разрешенных действий и условий для ресурсов.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d496273d844f1754e45b156422aad3e0927e0656
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519605"
---
# <a name="unifiedrolepermission-resource-type"></a>Тип ресурса Унифиедролепермиссион

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию разрешенных действий с ресурсами и условий, которые должны выполняться для вступления в силу действия. Действия с ресурсами — это задачи, которые могут быть перфомед для ресурса. Например, ресурс Application поддерживает действия с ресурсами "создание", "обновление", "удаление" и "Сброс пароля".

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedResourceActions|Коллекция строк| Набор задач, которые могут быть перфомед для ресурса. |
|установлен|String| Необязательные ограничения, которые должны выполняться для эффективного разрешения. |

### <a name="allowedresourceactions-property"></a>Свойство Алловедресаурцеактионс

Ниже приведена схема действий с ресурсами. 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
Пример: `microsoft.directory/applications/credentials/update`.  

- Namespace — службы, которые предоставляют задачу. Например, все задачи в Azure Active Directory используют пространство имен Microsoft. Directory.  
- Объект Entity — логические функции или компоненты, предоставляемые службой в Microsoft Graph. Например, приложения, субъекты служб или группы.
- Набор свойств — конкретные свойства или аспекты объекта, для которого предоставляется доступ. Например, `microsoft.directory/applications/authentication/read` предоставляет возможность чтения URL-адреса ответа, URL-адреса выхода и неявного свойства Flow для объекта **Application** в Azure AD. Ниже приведены зарезервированные имена для общих наборов свойств.  
  - Аллпропертиес — задает все свойства объекта, включая привилегированные свойства. Примеры включают `microsoft.directory/applications/allProperties/read` и `microsoft.directory/applications/allProperties/update`.
  - Basic — назначает общие свойства чтения, но исключает привилегированных. Например, `microsoft.directory/applications/basic/update` позволяет обновлять стандартные свойства, такие как отображаемое имя.
  - Standard — назначает общие свойства обновления, но исключает привилегированных. Например, `microsoft.directory/applications/standard/read`.
- Actions — операции, которые вы предоставляете. В большинстве случаев разрешения следует выражать в терминах CRUD или Аллтаскс. Сюда входят следующие действия:
  - Create — возможность создания нового экземпляра объекта.
  - Read — возможность считывания данного набора свойств (включая Аллпропертиес).
  - Update — возможность обновления набора свойств (включая Аллпропертиес).
  - Delete — возможность удаления данной сущности.
  - Аллтаскс — представляет все операции CRUD (создание, чтение, обновление и удаление). 

### <a name="condition-property"></a>свойство Condition
Условия определяют ограничения, которые должны выполняться. Например, требование, которое участник является владельцем целевого объекта. Ниже приведены поддерживаемые условия.

- Само: "@Subject. objectId = = @Resource. objectId"
- Owner: "@Subject. objectId Any_of @Resource. Owners"

Ниже приведен пример разрешения роли с условием.

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "@Subject.objectId Any_of @Resource.owners"
        }
    ]

```

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRolePermission",
  "baseType": null
}-->

```json
{
  "allowedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a>См. также

- [Разрешения роли администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles) — сведения о разрешениях для встроенных ролей каталогов.
- [Подтипы регистрации приложений и разрешения в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions) — сведения о разрешениях, доступных для пользовательских ролей каталога. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
