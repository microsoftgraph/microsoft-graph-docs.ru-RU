---
title: Тип ресурса ПрожектпартиЦипатион
description: Тип ресурса ПрожектпартиЦипатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 72d36f21a156fd6239dd8466808b1fe6ba2e6889
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078299"
---
# <a name="projectparticipation-resource-type"></a>Тип ресурса ПрожектпартиЦипатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о проектах, связанных с пользователем.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список проектов](../api/profile-list-projects.md)|Коллекция [прожектпартиЦипатион](../resources/projectparticipation.md)|Получение ресурсов ПрожектпартиЦипатион из свойства навигации Projects.|
|[Создание ПрожектпартиЦипатион](../api/profile-post-projects.md)|[прожектпартиЦипатион](../resources/projectparticipation.md)|Создание нового объекта ПрожектпартиЦипатион.|
|[Получение ПрожектпартиЦипатион](../api/projectparticipation-get.md)|[прожектпартиЦипатион](../resources/projectparticipation.md)|Чтение свойств и связей объекта [прожектпартиЦипатион](../resources/projectparticipation.md) .|
|[Обновление ПрожектпартиЦипатион](../api/projectparticipation-update.md)|[прожектпартиЦипатион](../resources/projectparticipation.md)|Обновление свойств объекта [прожектпартиЦипатион](../resources/projectparticipation.md) .|
|[Удаление ПрожектпартиЦипатион](../api/projectparticipation-delete.md)|Нет|Удаляет объект [прожектпартиЦипатион](../resources/projectparticipation.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, связанные с проектом пользователем (например, цифровое преобразование, гидростенд). |
|Клиенты|[компанидетаил](../resources/companydetail.md)|Содержит подробные сведения о клиенте, для которого выполнялся проект. |
|коллаборатионтагс|Коллекция String|Содержит теги сценариев, с которыми пользователь связан с интересом. Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .|
|коллег|Коллекция [релатедперсон](../resources/relatedperson.md)|Список людей, которые также работали над проектом. |
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|описаны|[поситиондетаил](../resources/positiondetail.md)|Содержит подробные сведения о роли пользователя в проекте.|
|displayName|String|Содержит понятное имя проекта.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|спонсорами|Коллекция [релатедперсон](../resources/relatedperson.md)|Пользователь или люди, которые спонсорируют проект.    |
## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation",
  "baseType": ""
}-->

```json
{
  "@odata.type": "#microsoft.graph.projectParticipation",
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
  "client": {
    "@odata.type": "microsoft.graph.companyDetail"
  },
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "sponsors": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "collaborationTags": [
    "String"
  ]
}
```


