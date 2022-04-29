---
title: тип ресурса запроса
description: Представляет сведения о запросе в PIM или userConsentRequests
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e8702ef1b0bc091e5d2e24e2808a86cefbd82b9f
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134396"
---
# <a name="request-resource-type"></a>тип ресурса запроса

Пространство имен: microsoft.graph

Представляет сведения о запросе в [PIM](privilegedidentitymanagementv3-overview.md) или [API запроса согласия](userconsentrequest.md) пользователя.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalId|String| Идентификатор утверждения запроса.  |
|completedDateTime|DateTimeOffset| Время даты завершения запроса. |
|createdBy|[identitySet](../resources/identityset.md)|Субъект, создавшего запрос.|
|createdDateTime|DateTimeOffset|Дата создания запроса.|
|Customdata|String|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Не используется.|
|id|String|Уникальный идентификатор объекта запроса. Наследуется от [сущности](../resources/entity.md).|
|status|String| Состояние запроса. Значение null не допускается. Возможные значения: `Canceled`, , `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`и `Revoked``ScheduleCreated`. Значение null не допускается. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.request",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.request",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

