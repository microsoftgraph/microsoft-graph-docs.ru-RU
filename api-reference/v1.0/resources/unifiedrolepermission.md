---
title: Тип ресурса unifiedRolePermission
description: Разрешение роли каталога — это коллекция разрешенных действий и условий ресурсов.
ms.localizationpriority: medium
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 66c28bff1d6204dbe1a19a75bf1b9c47de6b502e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671404"
---
# <a name="unifiedrolepermission-resource-type"></a>Тип ресурса unifiedRolePermission

Пространство имен: microsoft.graph

Представляет коллекцию разрешенных действий ресурсов и условий, которые должны быть выполнены, чтобы действие было разрешено. Действия с ресурсами — это задачи, которые можно выполнять с ресурсом. Например, ресурс приложения может поддерживать действия по созданию, обновлению, удалите и сбросу пароля.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedResourceActions|Коллекция строк| Набор задач, которые можно выполнить с ресурсом. Обязательный. |
|Состояние|String| Необязательные ограничения, которые должны быть выполнены, чтобы разрешение было эффективным. |
|excludedResourceActions|Коллекция String| Набор задач, которые могут не выполняться с ресурсом. Пока не поддерживается. |

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
Условия определяют ограничения, которые должны быть выполнены. Например, необходимо, чтобы субъект был владельцем целевого ресурса. Ниже приведены поддерживаемые условия.

- `Self`: "@Subject.objectId == @Resource.objectId"
- `Owner`: "@Subject.objectId Any_of @Resource.owners"

Ниже приведен пример разрешения роли с условием, что субъект является владельцем целевого ресурса.

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
  "@odata.type": "#microsoft.graph.unifiedRolePermission",
  "allowedResourceActions": ["String"],
  "excludedResourceActions": ["String"],
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