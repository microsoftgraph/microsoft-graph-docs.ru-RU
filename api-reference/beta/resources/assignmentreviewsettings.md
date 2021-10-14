---
title: тип ресурса assignmentReviewSettings
description: Тип assignmentReviewSettings, используемый для свойства accessReviewSettings политики назначения пакетов доступа, предоставляет дополнительные параметры, чтобы выбрать, кто должен просмотреть назначения пакетов доступа из этой политики, и как часто они должны быть рассмотрены.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7bb8afe847a9ceca9f11a54cc7f9c69a44ac0cde
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2021
ms.locfileid: "60290269"
---
# <a name="assignmentreviewsettings-resource-type"></a>тип ресурса assignmentReviewSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для **свойства accessReviewSettings** политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Предоставляет дополнительные параметры, чтобы выбрать, кто должен просмотреть назначения пакетов доступа из этой политики и как часто они должны быть рассмотрены.  

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| accessReviewTimeoutBehavior | [accessReviewTimeoutBehavior](#accessreviewtimeoutbehavior-values) | Решение по умолчанию применяться, если запрос не рассмотрен в течение периода, указанного в **durationInDays.** Возможные значения: `acceptAccessRecommendation` , `keepAccess` , и `removeAccess` `unknownFutureValue` . |
| durationInDays | Int32 | Количество дней, в течение которых рецензенты должны предоставлять входные данные.|
| isAccessRecommendationEnabled | Boolean | Указывает, следует ли отобразить рекомендации рецензенту. Значение по умолчанию `true` |
| isApprovalJustificationRequired | Boolean | Указывает, должен ли рецензент предоставить обоснование утверждения. Значение по умолчанию — `true`. |
| isEnabled| Boolean | Если это так, необходимо просмотреть доступ для назначений из этой политики. |
| recurrenceType | Строка | Интервал для повторения, например `monthly` или `quarterly` . |
| reviewerType | Строка | Кто должны быть предложены, чтобы сделать обзор, либо `Self` `Reviewers` или . |
| рецензенты | [коллекция userSet](userset.md) | Если это рецензентType, в этой коллекции указаны пользователи, которые будут рецензентами по ID или в качестве членов группы, используя коллекцию `Reviewers` [singleUser](singleuser.md) и [groupMembers](groupmembers.md). |
| startDateTime | DateTimeOffset | Когда должен начаться первый обзор. |

### <a name="accessreviewtimeoutbehavior-values"></a>значения accessReviewTimeoutBehavior

| Member | Описание |
|:---------------|:--------|:----------|
| acceptAccessRecommendation | Решение о проверке для принятия рекомендаций из обзора доступа к принятию и удалению доступа к пакету доступа. Общим правилом для рекомендаций AR является, если последний пользователь вошел более чем за 30 дней, рекомендуется удалить доступ к этому пользователю. |
| keepAccess | Решение о проверке — сохранить текущий доступ. |
| removeAccess | Решение об отзыве — удалить доступ к пакету доступа. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentReviewSettings",
  "isEnabled": "Boolean",
  "recurrenceType": "String",
  "reviewerType": "String",
  "startDateTime": "String (timestamp)",
  "durationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "isAccessRecommendationEnabled": "Boolean",
  "isApprovalJustificationRequired": "Boolean",
  "accessReviewTimeoutBehavior": "String"
}
```


