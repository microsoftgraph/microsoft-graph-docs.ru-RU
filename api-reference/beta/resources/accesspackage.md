---
title: Тип ресурса accessPackage
description: Пакет доступа определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e47b8076e70c5b7c792c0232c63ae9ce828ac146
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155645"
---
# <a name="accesspackage-resource-type"></a>Тип ресурса accessPackage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В службе управления правами [Azure AD](entitlementmanagement-root.md)пакет доступа определяет коллекции ролей ресурсов и политики предоставления доступа к этим ресурсам одним или более пользователями.  
Каждый пакет доступа ссылается на один каталог пакетов доступа и содержит ссылки на ресурсы из этого каталога через области ролей для определенных ресурсов, которые определяют доступ, который предоставляет пакет.  Пакет доступа также ссылается на политики назначения пакетов доступа, каждая из которых определяет, кто может запрашивать или кому назначено назначение пакета доступа.

Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на пакет доступа и политику назначения пакета доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackages](../api/accesspackage-list.md) | [Коллекция accessPackage](accesspackage.md) | Получить список объектов **accesspackage.** |
| [Создание accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | Создание объекта **accesspackage.** |
| [Get accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accesspackage.** |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage.** |
| [Удаление accessPackage](../api/accesspackage-delete.md) |Нет | Удаление **accesspackage**. |
| [Список accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Получить список объектов **accessPackageResourceRoleScope** для этого пакета доступа. |
| [Создание accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) |Нет | Создайте новый **объект accessPackageResourceRoleScope** для этого пакета доступа. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|catalogId|String|ИД каталога пакетов доступа, ссылаясь на этот пакет доступа. Только для чтения.|
|createdBy|String|UpN пользователя или удостоверения субъекта, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|description|String|Описание пакета доступа.|
|displayName|String|Отображаемого имени пакета доступа.|
|id|String| Только для чтения.|
|isHidden|Boolean|Является ли пакет доступа скрытым от запрашивателя.|
|isRoleScopesVisible|Boolean|Указывает, видны ли области ролей.|
|modifiedBy|String|Имя пользователя, который последним изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|[Коллекция accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Только для чтения. Допускается значение null.|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| Только для чтения. Допускается значение null.|
|accessPackageResourceRoleScopes|[Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)| Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


