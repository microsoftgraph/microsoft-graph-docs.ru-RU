---
title: Тип ресурса Персонинтерест
description: Тип ресурса Персонинтерест
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7071f089c7dbc9ff309dfc1d45628ef24c367567
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997965"
---
# <a name="personinterest-resource-type"></a>Тип ресурса Персонинтерест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип                         | Описание                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
|[Список интересов](../api/profile-list-interests.md)|Коллекция [персонинтерест](../resources/personinterest.md)|Получение ресурсов Персонинтерест из свойства навигации по интересам.|
|[Создание Персонинтерест](../api/profile-post-interests.md)|[персонинтерест](../resources/personinterest.md)|Создание нового объекта Персонинтерест.|
|[Получение Персонинтерест](../api/personinterest-get.md)|[персонинтерест](../resources/personinterest.md)|Чтение свойств и связей объекта [персонинтерест](../resources/personinterest.md) .|
|[Обновление Персонинтерест](../api/personinterest-update.md)|[персонинтерест](../resources/personinterest.md)|Обновление свойств объекта [персонинтерест](../resources/personinterest.md) .|
|[Удаление Персонинтерест](../api/personinterest-delete.md)|Нет|Удаляет объект [персонинтерест](../resources/personinterest.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, которые пользователь связал с интересом (например, персональный, реЦипиес). |
|коллаборатионтагс|Коллекция String|Содержит теги сценариев, с которыми пользователь связан с интересом. Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|description|String|Содержит описание интереса.|
|displayName|String|Содержит понятное имя для интереса.  |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl|String|Содержит ссылку на веб-страницу или ресурс, представляющие интерес. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
  "baseType": ""
}-->

```json
{
  "@odata.type": "#microsoft.graph.personInterest",
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
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```


