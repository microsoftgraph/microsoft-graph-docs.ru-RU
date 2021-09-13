---
title: тип ресурса itemAddress
description: тип ресурса itemAddress
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 72c48b2f96e60ab208d17aa4bb46dc7499d16728
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033401"
---
# <a name="itemaddress-resource-type"></a>тип ресурса itemAddress

Пространство имен: microsoft.graph

Представляет физический адрес и сведения о расположении, где найден адрес.

Наследует от [itemFacet](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Адреса списков](../api/profile-list-addresses.md)|[коллекция itemAddress](../resources/itemaddress.md)|Получите ресурсы itemAddress из свойства навигации адресов.|
|[Создание itemAddress](../api/profile-post-addresses.md)|[itemAddress](../resources/itemaddress.md)|Создание нового объекта itemAddress.|
|[Get itemAddress](../api/itemaddress-get.md)|[itemAddress](../resources/itemaddress.md)|Ознакомьтесь с свойствами и отношениями [объекта itemAddress.](../resources/itemaddress.md)|
|[Обновление itemAddress](../api/itemaddress-update.md)|[itemAddress](../resources/itemaddress.md)|Обновление свойств объекта [itemAddress.](../resources/itemaddress.md)|
|[Удаление itemAddress](../api/itemaddress-delete.md)|Нет|Удаляет объект [itemAddress.](../resources/itemaddress.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут видеть значения, содержащиеся в объекте. Унаследовано от [itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|подробные|[physicalAddress](../resources/physicaladdress.md)|Сведения о самом адресе.|
|displayName|String|Удобное имя, назначенное пользователю по этому адресу. |
|geoCoordinates|[geoCoordinates](../resources/geocoordinates.md)|Геокоординирует адрес.|
|id|String|Идентификатор, используемый для индивидуального обращения к объекту. Унаследованный от [сущности](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или модифицируют приложение. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили объект. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для создания объекта. Унаследовано от [itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникли, если синхронизированы с другой службы. Унаследовано от [itemFacet](../resources/itemfacet.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAddress",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAddress",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  }
}
```


