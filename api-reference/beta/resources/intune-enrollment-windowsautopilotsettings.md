---
title: Тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет учетную запись автопилота Windows для синхронизации данных с службой синхронизации данных устройств Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f6e65e2c898cbaaaf9d77b00cbf056d4cf369af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288630"
---
# <a name="windowsautopilotsettings-resource-type"></a>Тип ресурса windowsAutopilotSettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс windowsAutopilotSettings представляет учетную запись автопилота Windows для синхронизации данных с службой синхронизации данных устройств Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Чтение свойств и связей объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[Обновление windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Обновление свойств объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[Действие sync](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации данных в службе DDS.|
|ластмануалсинктригжердатетиме|DateTimeOffset|Дата и время последней синхронизации данных в службе DDS.|
|syncStatus|[виндовсаутопилотсинкстатус](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Указывает состояние синхронизации со службой синхронизации данных устройств (DDS). Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```




