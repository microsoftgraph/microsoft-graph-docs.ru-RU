---
title: тип ресурса teamworkDeviceOperation
description: Представляет сведения об операциях async, работающих на устройстве с Microsoft Teams с включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 513e18da8ed8432ce988c15f9737944d2493df3d
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262644"
---
# <a name="teamworkdeviceoperation-resource-type"></a>тип ресурса teamworkDeviceOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об операциях async, работающих на устройстве с [Microsoft Teams, включая](../resources/teamworkdevice.md) состояние операции. Любая операция async, запущенная на устройстве, создает **объект teamworkDeviceOperation** .

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список teamworkDeviceOperations](../api/teamworkdeviceoperation-list.md)|[коллекция teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Получите список объектов [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) и их свойств.|
|[Get teamworkDeviceOperation](../api/teamworkdeviceoperation-get.md)|[teamworkDeviceOperation](../resources/teamworkdeviceoperation.md)|Ознакомьтесь с свойствами и отношениями объекта [teamworkDeviceOperation](../resources/teamworkdeviceoperation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|Время, в течение которого операция достигла конечного состояния (например, `Successful`и `Failed``Cancelled`).|
|createdBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, создавшего операцию устройства.|
|createdDateTime|DateTimeOffset|Дата и время создания операции устройства.|
|error|[operationError](../resources/operationerror.md)|Сведения об ошибках доступны только в случае сбойного состояния.|
|id|String|Идентификатор документа. Наследуется [от сущности](../resources/entity.md).|
|lastActionBy|[identitySet](../resources/identityset.md)|Удостоверение пользователя, который в последний раз менял работу устройства.|
|lastActionDateTime|DateTimeOffset|Дата и время последней модификации операции устройства.|
|operationType|teamworkDeviceOperationType|Тип операции async на устройстве. Возможные значения: `deviceRestart`, , `configUpdate``deviceDiagnostics`, , `softwareUpdate`, `deviceManagementAgentConfigUpdate``remoteLogin`, `remoteLogout``unknownFutureValue`.|
|startedDateTime|DateTimeOffset|Время начала операции.|
|status|String|Текущий статус операции async, например, `Queued`, , `Scheduled`, `InProgress`, `Successful`и `Cancelled``Failed`.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceOperation",
  "completedDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.operationError"
  },
  "id": "String (identifier)",
  "lastActionBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastActionDateTime": "String (timestamp)",
  "operationType": "String",
  "startedDateTime": "String (timestamp)",
  "status": "String"
}
```

