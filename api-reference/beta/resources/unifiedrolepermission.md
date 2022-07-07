---
title: Тип ресурса unifiedRolePermission
description: Разрешение роли каталога — это коллекция разрешенных действий и условий ресурсов.
ms.localizationpriority: medium
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6ba2290c37e1543dd2eefd0de9baa75f460baa3a
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668666"
---
# <a name="unifiedrolepermission-resource-type"></a>Тип ресурса unifiedRolePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию разрешенных действий ресурсов и условий, которые должны быть выполнены, чтобы действие было эффективным. Действия с ресурсами — это задачи, которые можно выполнять с ресурсом. Например, ресурс приложения поддерживает действия по созданию, обновлению, удалите и сбросу ресурса пароля.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedResourceActions|Коллекция строк| Набор задач, которые можно выполнить с ресурсом. |
|Состояние|String| Необязательные ограничения, которые должны быть выполнены, чтобы разрешение было эффективным. |

### <a name="allowedresourceactions-property"></a>Свойство allowedResourceActions

Ниже приведена схема действий с ресурсами. 

```
{Namespace}/{Entity}/{PropertySet}/{Action}  
```
Пример: `microsoft.directory/applications/credentials/update`.  

- *{Namespace}* — службы, предоставляющие задачу. Например, все задачи в Azure Active Directory используют пространство имен `microsoft.directory`.  
- *{Entity}* — логические функции или компоненты, предоставляемые службой в Microsoft Graph. Например, `applications`или `servicePrincipals``groups`.
- *{PropertySet}* — необязательный параметр. Конкретные свойства или аспекты сущности, для которой предоставляется доступ. Например, предоставляет `microsoft.directory/applications/authentication/read` возможность чтения URL-адреса ответа, URL-адреса выхода и свойства неявного потока для  объекта приложения в Azure AD. Ниже перечислены зарезервированные имена для общих наборов свойств.  
  - `allProperties` — назначает все свойства сущности, включая привилегированные свойства. Примеры включают и `microsoft.directory/applications/allProperties/read` `microsoft.directory/applications/allProperties/update`.
  - `basic` — обозначает общие свойства чтения, но исключает привилегированные. Например, включает `microsoft.directory/applications/basic/update` возможность обновления стандартных свойств, таких как отображаемое имя.
  - `standard` — обозначает общие свойства обновления, но исключает привилегированные. Например, `microsoft.directory/applications/standard/read`.
- *{Actions}* — выполняемые операции. В большинстве случаев разрешения должны быть выражены с точки зрения операций CRUD или `allTasks`. Действия:
  - `create` — возможность создания нового экземпляра сущности.
  - `read` — возможность чтения заданного набора свойств (включая allProperties).
  - `update` — возможность обновления заданного набора свойств (включая allProperties).
  - `delete` — возможность удаления заданной сущности.
  - `allTasks` — представляет все операции CRUD (создание, чтение, обновление и удаление). 

### <a name="condition-property"></a>свойство condition
Условия определяют ограничения, которые должны быть выполнены. Например, необходимо, чтобы субъект был владельцем целевого объекта. Ниже приведены поддерживаемые условия.

- Self: "$ResourceIsSelf"
- Владелец: "$SubjectIsOwner"

Ниже приведен пример разрешения роли с условием.

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "$SubjectIsOwner"
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

- [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) — сведения о разрешениях для встроенных ролей каталога.
- [Подтипы и](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) разрешения регистрации приложений в Azure Active Directory — сведения о разрешениях, доступных для настраиваемых ролей каталогов. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
