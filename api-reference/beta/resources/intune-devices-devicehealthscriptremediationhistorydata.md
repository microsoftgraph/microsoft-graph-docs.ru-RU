---
title: Тип ресурса Девицехеалсскриптремедиатионхисторидата
description: Количество устройств, исправленных сценарием работоспособности устройства на заданную дату.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 396c52cbf797b0e0028e9f7ed71ca1e9fe05d34c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388504"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a>Тип ресурса Девицехеалсскриптремедиатионхисторидата

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество устройств, исправленных сценарием работоспособности устройства на заданную дату.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|date|Date|Дата исправления устройств с помощью сценария работоспособности устройства.|
|remediatedDeviceCount|Int32|Количество устройств, исправленных сценарием работоспособности устройства.|
|ноиссуедевицекаунт|Int32|Количество устройств, для которых было обнаружено отсутствие ошибок в сценарии работоспособности устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "<Unknown Primitive Type Edm.Date>",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```



