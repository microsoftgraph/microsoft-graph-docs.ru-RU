---
title: accessPackageAssignmentReviewSettings сложный тип
description: Используется для обзоров доступа к назначениям пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8deb20e147d9572911bc94aaec83750e8972592e
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608400"
---
# <a name="accesspackageassignmentreviewsettings-complex-type"></a>accessPackageAssignmentReviewSettings сложный тип

Пространство имен: microsoft.graph

Параметры в политике назначения пакетов доступа для [](accesspackageassignmentpolicy.md) отзывов о доступе к пакетам доступа, которые были сделаны с помощью этой политики. Предоставляет параметры для выбора рецензентов этих назначений и того, как часто эти назначения должны быть пересмотрены.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|expirationBehavior|accessReviewExpirationBehavior|Решение по умолчанию применяется, если доступ не будет рассмотрен. Допустимые значения: `keepAccess`, `removeAccess`, `acceptAccessRecommendation`, `unknownFutureValue`.|
|fallbackReviewers|[коллекция subjectSet](../resources/subjectset.md)|В этой коллекции указаны пользователи, которые будут рецензентами откатов, если основные рецензенты не отвечают.|
|isEnabled|Boolean|Если `true`для назначений с помощью этой политики требуется просмотреть доступ.|
|isRecommendationEnabled|Boolean|Указывает, следует ли отобразить рекомендации рецензенту. Значение по умолчанию — `true`.|
|isReviewerJustificationRequired|Boolean|Указывает, должен ли рецензент предоставить обоснование утверждения. Значение по умолчанию — `true`.|
|isSelfReview|Boolean|Указывает, могут ли директора пересматривать свои назначения.|
|primaryReviewers|[коллекция subjectSet](../resources/subjectset.md)|В этой коллекции указаны пользователи или группа пользователей, которые будут пересматривать назначения пакета доступа.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Когда должен начаться первый обзор и как часто он должен повториться.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentReviewSettings",
  "isEnabled": "Boolean",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  },
  "isSelfReview": "Boolean",
  "primaryReviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "expirationBehavior": "String",
  "isRecommendationEnabled": "Boolean",
  "isReviewerJustificationRequired": "Boolean"
}
```


