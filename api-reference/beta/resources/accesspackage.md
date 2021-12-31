---
title: тип ресурса accessPackage
description: Пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0f46825d8ae8dd1c5487a7c0f1f5b97d18337e87
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650631"
---
# <a name="accesspackage-resource-type"></a>тип ресурса accessPackage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-overview.md)пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.  

Каждый пакет доступа ссылается на единый каталог пакетов доступа и имеет ссылки на ресурсы из этого каталога с помощью областей ролей, определенных ресурсами, которые определяют доступ, который предоставляет пакет.  Пакет доступа также связывается с политиками назначения пакета доступа, каждая из которых определяет, кто может запрашивать или кому назначено назначение пакета доступа.

Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) который ссылается на политику назначения пакета доступа и пакета доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Пакеты доступа к спискам](../api/entitlementmanagement-list-accesspackages.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка **объектов accesspackage.** |
| [Создание accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | Создайте новый **объект accesspackage.** |
| [Получить accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | Чтение свойств и связей объекта **accesspackage.** |
| [Обновление accessPackage](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **accesspackage.** |
| [Удаление accessPackage](../api/accesspackage-delete.md) |Нет | Удаление **accesspackage**. |
| [Список accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Извлечение списка **объектов accessPackageResourceRoleScope** для этого пакета доступа. |
| [Создание accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) |Нет | Создайте новый **объект accessPackageResourceRoleScope** для этого пакета доступа. |
| [Список несовместимыхAccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка несовместимых объектов **accesspackage** для этого пакета доступа. |
| [Добавление accessPackage в несовместимыеAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | Нет | Добавьте ссылку, чтобы указать другой **пакет доступа** несовместим с указанным пакетом доступа. |
| [Удаление accessPackage из несовместимыхAccessPackages](../api/accesspackage-delete-incompatibleaccesspackage.md) | Нет | Удалить ссылку, которая указывала на **несовместимость accesspackage.** |
| [Несовместимые группы списка](../api/accesspackage-list-incompatiblegroups.md) | Коллекция [group](group.md) | Извлечение списка несовместимых **групповых** объектов для этого пакета доступа. |
| [Добавление группы в несовместимые Группы](../api/accesspackage-post-incompatiblegroup.md) | Нет | Добавьте ссылку, чтобы указать, что членство **в группе** несовместимо с указанным пакетом доступа. |
| [Удаление группы из несовместимых групп](../api/accesspackage-delete-incompatiblegroup.md) | Нет | Удалите ссылку, которая указывала, что членство **в** группе несовместимо.|
| [Список accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [коллекция accessPackage](accesspackage.md) | Извлечение списка объектов  **accesspackage,** которые перечисляют этот пакет доступа как несовместимые. |
|[filterByCurrentUser](../api/accesspackage-filterbycurrentuser.md)|[коллекция accessPackage](../resources/accesspackage.md)|Извлечение списка **объектов accessPackage,** фильтруемых на входе пользователя.|
| [getApplicablePolicyRequirements](../api/accesspackage-getapplicablepolicyrequirements.md) | [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) collection | Извлечение списка **объектов accessPackageAssignmentRequestRequirement** с требованиями запроса. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|catalogId|Строка|Идентификатор каталога пакетов доступа, ссылаясь на этот пакет доступа. Только для чтения.|
|createdBy|String|UserPrincipalName пользователя или удостоверения субъекта, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание пакета доступа.|
|displayName|Строка|Отображение имени пакета доступа. Поддерживает $filter ( `eq` , `contains` ).|
|id|String| Только для чтения.|
|isHidden|Логический|Скрыт ли пакет доступа от запросителя.|
|isRoleScopesVisible|Boolean|Указывает, видны ли области ролей.|
|modifiedBy|String|UserPrincipalName пользователя, который в последний раз изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |

## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection| Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|accessPackageCatalog|[accessPackageCatalog](accesspackagecatalog.md)| Только для чтения. Допускается значение null.|
|accessPackageResourceRoleScopes|[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)| Допускается значение null.|
| incompatibleAccessPackages | [коллекция accessPackage](accesspackagecatalog.md) | Пакеты доступа, которым назначены пользователи, не могут быть назначены этому пакету доступа. |
| accessPackagesIncompatibleWith | [коллекция accessPackage](accesspackagecatalog.md) | Пакеты доступа, несовместимые с этим пакетом. Только для чтения. |
| incompatibleGroups | Коллекция [group](group.md) | Группы, члены которых не могут быть назначены этому пакету доступа. |


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


