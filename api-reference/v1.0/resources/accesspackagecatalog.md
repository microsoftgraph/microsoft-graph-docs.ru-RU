---
title: тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: caf556556100da6d53447c9576eb1674a20c9b02
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242763"
---
# <a name="accesspackagecatalog-resource-type"></a>тип ресурса accessPackageCatalog

Пространство имен: microsoft.graph


В [управлении правами Azure AD](entitlementmanagement-root.md)каталог пакетов доступа — это контейнер для пакетов с нулевым или более доступом. Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для обеспечения доступа. Чтобы просмотреть или изменить членство ролей в [](unifiedroleassignment.md) каталоге, используйте API назначений ролей с поставщиком управления правами RBAC.



## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessPackageCatalogs](../api/entitlementmanagement-list-catalogs.md)|[коллекция accessPackageCatalog](accesspackagecatalog.md)|Извлечение списка объектов accessPackageCatalog. |
|[Создание accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md)|[accessPackageCatalog](accesspackagecatalog.md)|Создайте новый объект accessPackageCatalog. |
|[Получить accessPackageCatalog](../api/accesspackagecatalog-get.md)|[accessPackageCatalog](accesspackagecatalog.md)|Чтение свойств и связей объекта accessPackageCatalog. |
|[Обновление accessPackageCatalog](../api/accesspackagecatalog-update.md)|Нет|Обновление свойств объекта accessPackageCatalog. |
|[Удаление accessPackageCatalog](../api/accesspackagecatalog-delete.md)|Нет|Удаление accessPackageCatalog. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|catalogType|accessPackageCatalogType|Создается ли каталог пользователем или управлением правами. Допустимые значения: `userManaged`, `serviceDefault`, `serviceManaged`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения.|
|description|Строка|Описание каталога пакетов доступа.|
|displayName|Строка|Отображение имени каталога пакетов доступа.|
|id|String|Только для чтения.|
|isExternallyVisible|Boolean|Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|state|accessPackageCatalogState|Имеет `published` значение, если пакеты доступа доступны для управления. Допустимые значения: `unpublished`, `published`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackages|[коллекция accessPackage](accesspackage.md)|Пакеты доступа в этом каталоге. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageCatalog",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "catalogType": "String",
  "state": "String",
  "isExternallyVisible": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


