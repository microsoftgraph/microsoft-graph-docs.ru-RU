---
title: тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет собой Windows учетную запись автопилота для синхронизации данных с Windows службой синхронизации данных устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d9ab364d05384f9329f4dcad48ee6a93173cf978c0b58c4ff81a9a3e4b66819
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172905"
---
# <a name="windowsautopilotsettings-resource-type"></a>тип ресурса windowsAutopilotSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс windowsAutopilotSettings представляет собой Windows учетную запись автопилота для синхронизации данных с Windows службой синхронизации данных устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-get.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Чтение свойств и связей [объекта WindowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)|
|[Обновление windowsAutopilotSettings](../api/intune-enrollment-windowsautopilotsettings-update.md)|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Обновление свойств объекта [windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)|
|[Действие sync](../api/intune-enrollment-windowsautopilotsettings-sync.md)|Нет|Инициирует синхронизацию всех зарегистрированных устройств АвтоПилота из Магазина для бизнеса и других порталов. Если синхронизация будет успешной, это действие возвращает код ответа 204 Без контента. Если синхронизация уже продолжается, действие возвращает код ответа на конфликт 409.  Если это действие синхронизации вызвано в течение 10 минут после предыдущей синхронизации, действие возвращает код ответа 429 Too Many Requests.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|lastSyncDateTime|DateTimeOffset|Последнее время синхронизации данных со службой DDS.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Последнее время синхронизации данных со службой DDS.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Указывает состояние синхронизации со службой синхронизации данных устройств (DDS). Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.|

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




