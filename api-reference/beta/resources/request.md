---
title: тип ресурса запроса
description: Тип абстрактного объекта для моделирования рабочего процесса асинхронизированного запроса для создания, обновления и удаления объекта.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 871f2232e57bdd24aeff9842df699ea0601146eb
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509191"
---
# <a name="request-resource-type"></a>тип ресурса запроса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип абстрактного объекта для моделирования рабочего процесса асинхронизированного запроса для создания, обновления и удаления объекта.

Наследует [от сущности](entity.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalId|Строка|Идентификатор утверждения запроса.|
|completedDateTime|DateTimeOffset|Время завершения запроса.|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот запрос.|
|createdDateTime|DateTimeOffset|Время создания запроса.|
|customData|Строка|Свободное текстовое поле для определения настраиваемой информации для запроса. Не используется.|
|status|String|Состояние запроса. Значение null не допускается. Возможные значения: `Canceled`, , `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`и `Revoked``Provisioned``ScheduleCreated`. Значение null не допускается.|
|id|String|Идентификатор запроса. Только для чтения. Значение null не допускается. Наследуется от [сущности](entity.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|утверждение|[утверждение](../resources/approval.md)|Представляет объект утверждения, с который связан запрос.|

## <a name="json-representation"></a>Представление JSON
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

