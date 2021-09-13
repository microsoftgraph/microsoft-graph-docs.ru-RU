---
title: тип ресурса unifiedRolePermission
description: Разрешение роли каталога — это набор допустимых действий и условий ресурса.
ms.localizationpriority: medium
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 354d4be8875499553fdf2bdae4c0bb793997e158
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148524"
---
# <a name="unifiedrolepermission-resource-type"></a>тип ресурса unifiedRolePermission

Пространство имен: microsoft.graph

Представляет коллекцию допустимых действий ресурса и условия, которые должны быть выполнены для разрешенного действия. Действия ресурса — это задачи, которые можно выполнить на ресурсе. Например, ресурс приложения может поддерживать действия по созданию, обновлению, удалению и сбросу пароля.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedResourceActions|Коллекция строк| Набор задач, которые можно выполнить на ресурсе. Обязательно. |
|условие|String| Необязательные ограничения, которые должны быть выполнены, чтобы разрешение было эффективным. |
|excludedResourceActions|Коллекция String| Набор задач, которые могут не выполняться на ресурсе. Еще не поддерживается. |

### <a name="allowedresourceactions-property"></a>свойство allowedResourceActions

Ниже приводится схема действий с ресурсами: 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
Пример: `microsoft.directory/applications/credentials/update`.  

- Namespace — службы, которые раскрывают задачу. Например, все задачи в Azure Active Directory использовать пространство имен microsoft.directory.  
- Entity — логические функции или компоненты, открытые службой в Microsoft Graph. Например, приложения, servicePrincipals или группы.
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
Условия определяют ограничения, которые должны быть выполнены. Например, требование о том, чтобы директор был владельцем целевого ресурса. Ниже следующую поддержку условий:

- `Self`: "@Subject.objectId == @Resource.objectId"
- `Owner`: "@Subject.objectId Any_of @Resource.owners"

Ниже приводится пример разрешения на роль с условием, что директором является владелец целевого ресурса.

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