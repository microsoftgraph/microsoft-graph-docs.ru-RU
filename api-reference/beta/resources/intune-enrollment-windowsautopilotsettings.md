---
title: Тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет учетную запись Windows автопилот данных синхронизации со службой синхронизации данных устройства Windows.
ms.openlocfilehash: 41caab7578be08a56ecad94bbae11c43945037c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078851"
---
# <a name="windowsautopilotsettings-resource-type"></a>Тип ресурса windowsAutopilotSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс windowsAutopilotSettings представляет учетную запись Windows автопилот данных синхронизации со службой синхронизации данных устройства Windows.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Чтение свойства и связи объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[Обновление windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Обновление свойства объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .|
|[Действие sync](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|lastSyncDateTime|DateTimeOffset|Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Указывает состояние синхронизации со службой синхронизации (набору доменов Обнаружения) данных устройства. Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.|

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





