---
title: Тип ресурса personInterest
description: Тип ресурса personInterest
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0b635ab19f4cda9985de05e317316579ad60f7b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161399"
---
# <a name="personinterest-resource-type"></a>Тип ресурса personInterest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет подробные сведения об интересах, которые пользователь связал с собой в различных службах.

Наследуется [от itemFacet.](itemfacet.md)

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип                         | Описание                                                           |
|:----------------------------------------------------------|:------------------------------------|:----------------------------------------------------------------------|
|[Список интересов](../api/profile-list-interests.md)|[Коллекция personInterest](../resources/personinterest.md)|Получите ресурсы personInterest из свойства навигации по интересам.|
|[Создание personInterest](../api/profile-post-interests.md)|[personInterest](../resources/personinterest.md)|Создание объекта personInterest.|
|[Get personInterest](../api/personinterest-get.md)|[personInterest](../resources/personinterest.md)|Чтение свойств и связей объекта [personInterest.](../resources/personinterest.md)|
|[Обновление personInterest](../api/personinterest-update.md)|[personInterest](../resources/personinterest.md)|Обновление свойств объекта [personInterest.](../resources/personinterest.md)|
|[Удаление personInterest](../api/personinterest-delete.md)|Нет|Удаляет объект [personInterest.](../resources/personinterest.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется [от itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, связанные пользователем с интересом (например, персональные, высмеи). |
|collaborationTags|Коллекция String|Содержит теги сценария работы, которые пользователь связал с интересом. Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , , `wantsToLearn` `wantsToImprove` .|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Наследуется [от itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для времени создания сущности. Наследуется [от itemFacet](../resources/itemfacet.md).|
|description|String|Содержит описание интерес.|
|displayName|String|Содержит удобное имя для интересуя вас.  |
|id|String|Идентификатор, используемый для индивидуального обращения к объекту. Наследуется [от объекта](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если сущность создается или изменяется приложением. Наследуется [от itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили сущность. Наследуется [от itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для времени создания сущности. Наследуется [от itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникают, если синхронизированы из другой службы. Наследуется [от itemFacet](../resources/itemfacet.md).|
|webUrl|String|Содержит ссылку на веб-страницу или ресурс о интересе. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest"
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


