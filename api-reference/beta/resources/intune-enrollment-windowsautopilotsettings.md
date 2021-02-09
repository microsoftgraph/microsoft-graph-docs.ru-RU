---
title: Тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет учетную запись Windows Autopilot для синхронизации данных со службой синхронизации данных устройств с Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e49191d204a040327c510606c6ca8186644beb7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159530"
---
# <a name="windowsautopilotsettings-resource-type"></a>Тип ресурса windowsAutopilotSettings

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс windowsAutopilotSettings представляет учетную запись Windows Autopilot для синхронизации данных со службой синхронизации данных устройств с Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Чтение свойств и связей объекта [windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)|
|[Обновление windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Обновление свойств объекта [windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)|
|[Действие sync](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Нет|Инициирует синхронизацию всех зарегистрированных AutoPilot устройств из Магазина для бизнеса и других порталов. Если синхронизация прошла успешно, это действие возвращает код отклика "204 Без содержимого". Если синхронизация уже идет, действие возвращает код ответа на конфликт 409.  Если это действие синхронизации вызвано в течение 10 минут после предыдущей синхронизации, это действие возвращает код ответа 429 Too Many Requests.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|lastSyncDateTime|DateTimeOffset|Время последней даты синхронизации данных со службой DDS.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Время последней синхронизации данных со службой DDS.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Указывает состояние синхронизации со службой синхронизации данных устройства (DDS). Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.|

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




