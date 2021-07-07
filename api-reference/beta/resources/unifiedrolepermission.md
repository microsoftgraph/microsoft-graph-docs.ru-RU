---
title: тип ресурса unifiedRolePermission
description: Разрешение роли каталога — это набор допустимых действий и условий ресурса.
localization_priority: Normal
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6fc799fec39eaa209ac8e74b02743cf84e76a51a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316492"
---
# <a name="unifiedrolepermission-resource-type"></a>тип ресурса unifiedRolePermission

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию допустимых действий ресурса и условия, которые должны быть выполнены для эффективного действия. Действия ресурса — это задачи, которые можно выполнить на ресурсе. Например, ресурс приложения поддерживает создание, обновление, удаление и сброс действий ресурса паролей.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedResourceActions|Коллекция строк| Набор задач, которые можно выполнить на ресурсе. |
|условие|String| Необязательные ограничения, которые должны быть выполнены, чтобы разрешение было эффективным. |

### <a name="allowedresourceactions-property"></a>свойство allowedResourceActions

Ниже приводится схема действий с ресурсами: 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
Пример: `microsoft.directory/applications/credentials/update`.  

- Namespace — службы, которые раскрывают задачу. Например, все задачи в Azure Active Directory использовать пространство имен microsoft.directory.  
- Entity — логические функции или компоненты, открытые службой в Microsoft Graph. Например, приложения, основные службы или группы.
- PropertySet — конкретные свойства или аспекты объекта, для которого предоставляется доступ. Например, предоставляется возможность чтения URL-адреса ответа, URL-адреса входа и неявного потока на объекте приложения `microsoft.directory/applications/authentication/read` в Azure  AD. Для общих наборов свойств зарезервированы следующие имена:  
  - allProperties — назначает все свойства объекта, включая привилегированные свойства. Примеры включают `microsoft.directory/applications/allProperties/read` и `microsoft.directory/applications/allProperties/update` .
  - basic — назначает общие свойства чтения, но исключает привилегированные свойства. Например, включает возможность обновления стандартных свойств, `microsoft.directory/applications/basic/update` таких как имя отображения.
  - стандартный . Назначает общие свойства обновления, но исключает привилегированные. Например, `microsoft.directory/applications/standard/read`.
- Действия — операции, которые будут предоставлены. В большинстве обстоятельств разрешения должны быть выражены с точки зрения CRUD или allTasks. Действия включают:
  - Create — возможность создания нового экземпляра объекта.
  - Чтение . Возможность чтения заданного набора свойств (включая allProperties).
  - Обновление . Возможность обновления данного набора свойств (включая allProperties).
  - Удаление — возможность удаления данного объекта.
  - AllTasks — представляет все операции CRUD (создание, чтение, обновление и удаление). 

### <a name="condition-property"></a>свойство condition
Условия определяют ограничения, которые должны быть выполнены. Например, требование о том, чтобы директор был "владельцем" целевой группы. Ниже следующую поддержку условий:

- Self: "$ResourceIsSelf"
- Владелец: "$SubjectIsOwner"

Ниже приводится пример разрешения на роль с условием.

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

- [Разрешения на роль](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) администратора в Azure Active Directory - Сведения о разрешениях для встроенных ролей каталога.
- [Подтипы](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) и разрешения регистрации приложений в Azure Active Directory - Сведения о разрешениях, доступных для пользовательских ролей каталога. 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
