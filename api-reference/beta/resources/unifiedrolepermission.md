---
title: Тип ресурса unifiedRolePermission
description: Разрешение роли каталога — это коллекция разрешенных действий и условий ресурсов.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 45c59567e8926e8ae7fc2429939b2491a8237782
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874286"
---
# <a name="unifiedrolepermission-resource-type"></a>Тип ресурса unifiedRolePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию разрешенных действий с ресурсами и условия, которые должны быть выполнены, чтобы действие было эффективным. Действия с ресурсами — это задачи, которые могут быть перенаучены для ресурса. Например, ресурс приложения поддерживает действия по созданию, обновлению, удалению и сбросу ресурсов паролей.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedResourceActions|Коллекция строк| Набор задач, которые можно выполнить с ресурсом. |
|condition|String| Необязательные ограничения, которые должны быть выполнены, чтобы разрешение было эффективным. |

### <a name="allowedresourceactions-property"></a>Свойство allowedResourceActions

Ниже приводится схема действий с ресурсами. 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
Пример: `microsoft.directory/applications/credentials/update`.  

- Пространство имен — службы, которые предоставляет задачу. Например, все задачи в Azure Active Directory используют пространство имен microsoft.directory.  
- Сущность — логические функции или компоненты, которые компоненты компоненты, компоненты, которые компоненты службы в Microsoft Graph. Например, приложения, основные службы или группы.
- PropertySet — конкретные свойства или аспекты сущности, для которой предоставляется доступ. Например, предоставляет возможность чтения URL-адреса ответа, URL-адреса для входа и неявного свойства потока в объекте приложения `microsoft.directory/applications/authentication/read` в Azure  AD. Для общих наборов свойств зарезервированы следующие имена:  
  - allProperties — назначает все свойства сущности, включая привилегированные свойства. Примеры: `microsoft.directory/applications/allProperties/read` и `microsoft.directory/applications/allProperties/update` .
  - basic — назначает общие свойства чтения, но исключает привилегированные свойства. Например, включает возможность обновления стандартных свойств, таких как `microsoft.directory/applications/basic/update` отображаемая имя.
  - standard — назначает общие свойства обновления, но исключает привилегированные свойства. Например, `microsoft.directory/applications/standard/read`.
- Действия — предоставленные операции. В большинстве ситуаций разрешения должны быть выражены с точки зрения CRUD или allTasks. К действиям относятся:
  - Create — возможность создания нового экземпляра сущности.
  - Чтение — возможность чтения заданного набора свойств (включая allProperties).
  - Update — возможность обновления заданного набора свойств (включая allProperties).
  - Delete — возможность удаления заданного объекта.
  - AllTasks — представляет все операции CRUD (создание, чтение, обновление и удаление). 

### <a name="condition-property"></a>свойство condition
Условия определяют ограничения, которые должны быть выполнены. Например, требование, что основной объект является "владельцем" целевого сайта. Поддерживаются следующие условия:

- Self: "@Subject.objectId == @Resource.objectId"
- Владелец: "@Subject.objectId Any_of @Resource.owners"

Ниже приводится пример разрешения роли с условием.

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

- [Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) — сведения о разрешениях для встроенных ролей каталога.
- [Подтипы и](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) разрешения регистрации приложений в Azure Active Directory — сведения о разрешениях, доступных для настраиваемой роли каталога. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->