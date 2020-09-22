---
title: Тип ресурса СкиллпрофиЦиенци
description: Тип ресурса СкиллпрофиЦиенци
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: d01c9fe6c4171c16d96e5b81eb8537ea0cbeb1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997678"
---
# <a name="skillproficiency-resource-type"></a>Тип ресурса СкиллпрофиЦиенци

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о навыках, связанных с пользователем в различных службах.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы
 
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список навыков](../api/profile-list-skills.md)|Коллекция [скиллпрофиЦиенци](../resources/skillproficiency.md)|Получение ресурсов СкиллпрофиЦиенци из свойства навигации по навыкам.|
|[Создание СкиллпрофиЦиенци ](../api/profile-post-skills.md)|[скиллпрофиЦиенци](../resources/skillproficiency.md)|Создание нового объекта СкиллпрофиЦиенци.|
|[Получение СкиллпрофиЦиенци](../api/skillproficiency-get.md)|[скиллпрофиЦиенци](../resources/skillproficiency.md)|Чтение свойств и связей объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) .|
|[Обновление СкиллпрофиЦиенци](../api/skillproficiency-update.md)|[скиллпрофиЦиенци](../resources/skillproficiency.md)|Обновление свойств объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) .|
|[Удаление СкиллпрофиЦиенци](../api/skillproficiency-delete.md)|Нет|Удаляет объект [скиллпрофиЦиенци](../resources/skillproficiency.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный). |
|коллаборатионтагс|Коллекция String|Содержит теги сценариев, с которыми пользователь связан с интересом. Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|displayName|String|Содержит понятное имя для навыка. |
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|навыки|скиллпрофиЦиенцилевел|Сведения о пользователях, которые подключают этот навык. Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|webUrl|String|Содержит ссылку на источник информации о навыке. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skillProficiency",
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
  "displayName": "String",
  "proficiency": "String",
  "webUrl": "String",
  "collaborationTags": [
    "String"
  ]
}
```

