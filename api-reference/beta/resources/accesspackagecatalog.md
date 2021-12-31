---
title: тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5d6eb82a55e21469ea1f0169f0a589fd4f449d15
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650512"
---
# <a name="accesspackagecatalog-resource-type"></a>тип ресурса accessPackageCatalog

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-overview.md)каталог пакетов доступа — это контейнер для пакетов с нулевым или более доступом. Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для обеспечения доступа. Чтобы просмотреть или изменить членство ролей в [](unifiedroleassignment.md) каталоге, используйте API назначений ролей с поставщиком управления правами RBAC.



## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [коллекция accessPackageCatalog](accesspackagecatalog.md) | Извлечение списка объектов accesspackagecatalog. |
| [Создание accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создайте новый объект accessPackageCatalog. |
| [Получить accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта accessPackageCatalog. |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта accessPackageCatalog. |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление accessPackageCatalog. |
| [Ресурсы accessPackageCatalog списка](../api/accesspackagecatalog-list-accesspackageresources.md) | [коллекция accessPackageResource](accesspackageresource.md) | Извлечение списка объектов accessPackageResource в каталоге. |
| [Роли ресурсов accessPackageCatalog в списке](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Извлечение списка объектов accessPackageResourceRole для ресурсов в каталоге. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|catalogStatus|Строка|Имеет `Published` значение, если пакеты доступа доступны для управления.|
|catalogType|Строка|Один `UserManaged` из или `ServiceDefault` . |
|createdBy|String|UPN пользователя, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание каталога пакетов доступа.|
|displayName|Строка|Отображение имени каталога пакетов доступа. Поддерживает `$filter` (`eq`, `contains`).|
|id|String| Только для чтения.|
|isExternallyVisible|Boolean|Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.|
|modifiedBy|Строка|UpN пользователя, который в последний раз изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |


## <a name="relationships"></a>Отношения

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackages|[коллекция accessPackage](accesspackage.md)| Пакеты доступа в этом каталоге. Только для чтения. Допускается значение null. Поддерживает `$expand`.|
|accessPackageResources|[коллекция accessPackageResource](accesspackageresource.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
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
  "description": "accessPackageCatalog resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

