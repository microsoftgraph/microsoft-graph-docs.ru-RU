---
title: тип ресурса запроса
description: Представляет сведения о запросе в PIM или userConsentRequests.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 72a52ce4911dc85a5d4f954cdc48e62ad8f1f9c2
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65897960"
---
# <a name="request-resource-type"></a>тип ресурса запроса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о запросе в [PIM](privilegedidentitymanagementv3-overview.md) или [API запроса согласия](userconsentrequest.md) пользователя.

Наследует [от сущности](../resources/entity.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalId|Строка| Идентификатор утверждения запроса.  |
|completedDateTime|DateTimeOffset| Время даты завершения запроса. |
|createdBy|[identitySet](../resources/identityset.md)|Субъект, создавшего запрос.|
|createdDateTime|DateTimeOffset|Дата создания запроса.|
|Customdata|Строка|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Не используется.|
|id|Строка|Уникальный идентификатор объекта запроса. Наследуется от [сущности](../resources/entity.md).|
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