---
title: Тип ресурса Персонвебсите
description: Тип ресурса Персонвебсите
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 3b480370309b6c843359a711ff27307c4d6e41e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997916"
---
# <a name="personwebsite-resource-type"></a>Тип ресурса Персонвебсите

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список веб-сайтов](../api/profile-list-websites.md)|Коллекция [персонвебсите](../resources/personwebsite.md)|Получение ресурсов Персонвебсите из свойства навигации веб-сайтов.|
|[Создание Персонвебсите](../api/profile-post-websites.md)|[персонвебсите](../resources/personwebsite.md)|Создание нового объекта Персонвебсите.|
|[Получение Персонвебсите](../api/personwebsite-get.md)|[персонвебсите](../resources/personwebsite.md)|Чтение свойств и связей объекта [персонвебсите](../resources/personwebsite.md) .|
|[Обновление Персонвебсите](../api/personwebsite-update.md)|[персонвебсите](../resources/personwebsite.md)|Обновление свойств объекта [персонвебсите](../resources/personwebsite.md) .|
|[Удаление Персонвебсите](../api/personwebsite-delete.md)|Нет|Удаляет объект [персонвебсите](../resources/personwebsite.md) .|

## <a name="properties"></a>Свойства

| Свойство     | Тип              | Описание                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|categories    |Коллекция String  | Содержит категории, связанные с веб-сайтом пользователя (например, персональный, рецепты).  |
|description   |String             | Содержит описание веб-сайта.                                                        |
|displayName   |String             | Содержит понятное имя для веб-сайта.                                                     |
|webUrl        |String             | Содержит ссылку на сам веб-сайт.                                                        |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, связанные с веб-сайтом пользователя (например, персональный, рецепты).|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description|String|Содержит описание веб-сайта.|
|displayName|String|Содержит понятное имя для веб-сайта.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl|String|Содержит ссылку на сам веб-сайт.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personWebsite",
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
  "categories": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```


