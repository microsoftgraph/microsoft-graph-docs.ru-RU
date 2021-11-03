---
title: тип ресурса запроса
description: Тип абстрактного объекта для моделирования рабочего процесса асинхронизированного запроса для создания, обновления и удаления объекта.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fad1d480fbb792ca63b05ddfe8507b2ede9d54e8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695253"
---
# <a name="request-resource-type"></a>тип ресурса запроса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип абстрактного объекта для моделирования рабочего процесса асинхронизированного запроса для создания, обновления и удаления объекта.

Наследует от [объекта](entity.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalId|String|Идентификатор утверждения запроса.|
|completedDateTime|DateTimeOffset|Время завершения запроса.|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот запрос.|
|createdDateTime|DateTimeOffset|Время создания запроса.|
|customData|String|Свободное текстовое поле для определения настраиваемой информации для запроса. Не используется.|
|status|String|Состояние запроса. Значение null не допускается. Возможные значения: `Canceled` `Denied` , , , , , , , , `Failed` и `Granted` `PendingAdminDecision` `PendingApproval` `PendingProvisioning` `PendingScheduleCreation` `Provisioned` `Revoked` `ScheduleCreated` . Значение null не допускается.|
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

