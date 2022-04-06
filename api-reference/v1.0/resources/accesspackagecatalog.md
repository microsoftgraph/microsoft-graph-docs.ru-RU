---
title: тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 556216ac7c7b51e18b2a918ccde63b5f730bf7d0
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477561"
---
# <a name="accesspackagecatalog-resource-type"></a>тип ресурса accessPackageCatalog

Пространство имен: microsoft.graph


В [управлении правами Azure AD](entitlementmanagement-overview.md) каталог пакетов доступа — это контейнер для пакетов с нулевым или более доступом. Управление правами Azure AD включает встроенный каталог с именем **General**.

Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для обеспечения доступа. Чтобы просмотреть или изменить членство ролей в каталоге, используйте API назначений ролей с поставщиком управления правами RBAC.[](unifiedroleassignment.md)



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
|state|accessPackageCatalogState|Имеет значение, `published` если пакеты доступа доступны для управления. Допустимые значения: `unpublished`, `published`, `unknownFutureValue`.|

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


