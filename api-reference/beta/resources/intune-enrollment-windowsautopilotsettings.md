---
title: тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет собой Windows учетную запись автопилота для синхронизации данных с Windows службой синхронизации данных устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d79155c3642eee237fd4bda53ecb6650f5cfbe7e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039961"
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



