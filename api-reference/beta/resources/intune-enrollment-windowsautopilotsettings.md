---
title: Тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет учетную запись автопилота Windows для синхронизации данных с службой синхронизации данных устройств Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7882a522eb3e3adcf9ebdf24e2b8f820b0f3581
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547048"
---
# <a name="windowsautopilotsettings-resource-type"></a>Тип ресурса windowsAutopilotSettings

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|Ластмануалсинктригжердатетиме|DateTimeOffset|Дата и время последней синхронизации данных в службе DDS.|
|syncStatus|[Виндовсаутопилотсинкстатус](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Указывает состояние синхронизации со службой синхронизации данных устройств (DDS). Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.|

## <a name="relationships"></a>Отношения
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





