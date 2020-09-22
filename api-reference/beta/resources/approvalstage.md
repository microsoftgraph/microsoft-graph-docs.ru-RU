---
title: сложный тип Аппровалстаже
description: Используется для свойства Аппровалстажес параметров утверждения в свойстве Рекуестаппровалсеттингс политики назначения пакетов Access. Указывает основных, резервных и эскалациых утверждающих каждого этапа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: df7e9ce4491ea7a887b79f79d354c9099ea9f5d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050149"
---
# <a name="approvalstage-complex-type"></a>сложный тип Аппровалстаже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для свойства **аппровалстажес** параметров утверждения в свойстве **рекуестаппровалсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Указывает основных, резервных и эскалациых утверждающих каждого этапа.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| аппровалстажетимеаутиндайс |Int32 | Количество дней, в течение которых запрос может находиться в состоянии ожидания ответа, прежде чем он будет автоматически отклонен. |
| исаппровержустификатионрекуиред |Boolean | Указывает, является ли утверждающий обязательным для предоставления обоснования для утверждения запроса. |
| исескалатионенаблед |Boolean | Если задано значение true, на этом этапе утверждения настраивается один или несколько утверждающих. |
| ескалатионтимеинминутес |Int32 | Если требуется эскалация, время, в течение которого запрос может отреагировать от основного утверждающего лица. |
| примаряппроверс | Коллекция [User](userset.md) Collection| Пользователи, которые будут запрашивать разрешение на утверждение запросов. Коллекция объектов [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md) и [екстерналспонсорс](externalsponsors.md). |
| ескалатионаппроверс | Коллекция [User](userset.md) Collection| Если распространение включено и основные утверждающие не отвечают на время эскалации, Ескалатионаппроверс — это пользователи, которым будет предложено утвердить запросы. Это может быть коллекция [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md) и [екстерналспонсорс](externalsponsors.md).|



## <a name="json-representation"></a>Представление JSON

Ниже представлено представление объекта стадии утверждения запроса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage",
  "baseType": ""
}-->

```json

{
    "approvalStageTimeOutInDays": 14,
    "isApproverJustificationRequired": true,
    "isEscalationEnabled": true,
    "escalationTimeInMinutes": 11520,
    "primaryApprovers": [{"@odata.type": "microsoft.graph.userSet"}],
    "escalationApprovers": [{"@odata.type": "microsoft.graph.userSet"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


