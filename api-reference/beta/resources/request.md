---
title: тип ресурса запроса
description: Абстрактный тип сущности для моделирования асинхронного рабочего процесса запроса для создания, обновления и удаления объекта.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e75c2d632356fceffaf432fc4def204e837c9bc
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399399"
---
# <a name="request-resource-type"></a>тип ресурса запроса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип сущности для моделирования асинхронного рабочего процесса запроса для создания, обновления и удаления объекта.

Наследует [от сущности](entity.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalId|String|Идентификатор утверждения запроса.|
|completedDateTime|DateTimeOffset|Время даты завершения запроса.|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот запрос.|
|createdDateTime|DateTimeOffset|Дата создания запроса.|
|Customdata|String|Поле "Бесплатный текст" для определения любых пользовательских данных для запроса. Не используется.|
|status|String|Состояние запроса. Значение null не допускается. Возможные значения: `Canceled`, , `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`и `Revoked``ScheduleCreated`. Значение null не допускается.|
|id|String|Идентификатор запроса. Только для чтения. Значение null не допускается. Наследуется от [сущности](entity.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|утверждение|[утверждение](../resources/approval.md)|Представляет объект утверждения, с котором связан запрос.|

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
  "approvalId": "String (identifier)",
  "completedDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "customData": "String",
  "status": "String",
}
```

