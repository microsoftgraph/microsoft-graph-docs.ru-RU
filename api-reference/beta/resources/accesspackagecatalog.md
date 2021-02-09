---
title: Тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97c683ca47f453efdcd267839b3a2239a400db66
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158634"
---
# <a name="accesspackagecatalog-resource-type"></a>Тип ресурса accessPackageCatalog

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [службе управления правами Azure AD](entitlementmanagement-root.md)каталог пакетов доступа является контейнером для пакетов доступа с нуля или более.  Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для предоставления доступа.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [Коллекция accessPackageCatalog](accesspackagecatalog.md) | Получить список объектов accesspackagecatalog. |
| [Создание accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | Создание объекта accessPackageCatalog. |
| [Get accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | Чтение свойств и связей объекта accessPackageCatalog. |
| [Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта accessPackageCatalog. |
| [Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | Удаление accessPackageCatalog. |
| [Список ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresources.md) | [Коллекция accessPackageResource](accesspackageresource.md) | Получить список объектов accessPackageResource в каталоге. |
| [Список ролей ресурсов accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Коллекция accessPackageResourceRole](accesspackageresourcerole.md) | Получить список объектов accessPackageResourceRole для ресурсов в каталоге. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|catalogStatus|String|Имеет `Published` значение, если пакеты доступа доступны для управления.|
|catalogType|String|Один из `UserManaged` или `ServiceDefault` . |
|createdBy|String|Имя пользователя, создавшего этот ресурс. Только для чтения.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|description|String|Описание каталога пакетов доступа.|
|displayName|String|Отображаемого имени каталога пакетов доступа.|
|id|String| Только для чтения.|
|isExternallyVisible|Boolean|Могут ли пользователи за пределами клиента запрашивать пакеты доступа в этом каталоге.|
|modifiedBy|String|Имя пользователя, который последним изменил этот ресурс. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackages|[Коллекция accessPackage](accesspackage.md)| Пакеты доступа в этом каталоге. Только для чтения. Допускается значение null.|
|accessPackageResources|[Коллекция accessPackageResource](accesspackageresource.md)| Только для чтения. Допускается значение null.|

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


