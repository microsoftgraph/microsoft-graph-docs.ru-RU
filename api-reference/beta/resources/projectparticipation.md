---
title: Тип ресурса projectParticipation
description: Тип ресурса projectParticipation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1d349b33dc3325451e97d055c178082676b48de3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156366"
---
# <a name="projectparticipation-resource-type"></a>Тип ресурса projectParticipation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подробные сведения о проектах, связанных с пользователем.

Наследуется от [itemFacet.](itemfacet.md)

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список проектов](../api/profile-list-projects.md)|[Коллекция projectParticipation](../resources/projectparticipation.md)|Получите ресурсы projectParticipation из свойства навигации проектов.|
|[Создание projectParticipation](../api/profile-post-projects.md)|[projectParticipation](../resources/projectparticipation.md)|Создание объекта projectParticipation.|
|[Get projectParticipation](../api/projectparticipation-get.md)|[projectParticipation](../resources/projectparticipation.md)|Чтение свойств и связей объекта [projectParticipation.](../resources/projectparticipation.md)|
|[Обновление projectParticipation](../api/projectparticipation-update.md)|[projectParticipation](../resources/projectparticipation.md)|Обновление свойств объекта [projectParticipation.](../resources/projectparticipation.md)|
|[Удаление projectParticipation](../api/projectparticipation-delete.md)|Нет|Удаляет объект [projectParticipation.](../resources/projectparticipation.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedAudiences|String|Аудитории, которые могут видеть значения, содержащиеся в объекте. Наследуется [от itemFacet](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|categories|Коллекция String|Содержит категории, связанные с проектом пользователем (например, цифровая трансформация, оснастка). |
|client|[companyDetail](../resources/companydetail.md)|Содержит подробные сведения о клиенте, для который был проект. |
|collaborationTags|Коллекция String|Содержит теги сценария работы, которые пользователь связал с интересом. Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , , `wantsToLearn` `wantsToImprove` .|
|colleagues|[коллекция relatedPerson](../resources/relatedperson.md)|Перечисляет людей, которые также работали над проектом. |
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создав объект. Наследуется [от itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет dateTimeOffset для времени создания сущности. Наследуется [от itemFacet](../resources/itemfacet.md).|
|detail|[positionDetail](../resources/positiondetail.md)|Содержит сведения о роли пользователя в проекте.|
|displayName|String|Содержит удобное имя проекта.|
|id|String|Идентификатор, используемый для индивидуального обращения к объекту. Наследуется [от объекта](../resources/entity.md)|
|вывод|[inferenceData](../resources/inferencedata.md)|Содержит сведения о выводе, если сущность создается или изменяется приложением. Наследуется [от itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которые в последний раз изменили сущность. Наследуется [от itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет dateTimeOffset для времени создания сущности. Наследуется [от itemFacet](../resources/itemfacet.md).|
|source|[personDataSource](../resources/persondatasource.md)|Где значения возникают, если синхронизированы из другой службы. Наследуется [от itemFacet](../resources/itemfacet.md).|
|sponsors|[коллекция relatedPerson](../resources/relatedperson.md)|Лицо или люди, которые спонсировали проект.    |
## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation"
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


