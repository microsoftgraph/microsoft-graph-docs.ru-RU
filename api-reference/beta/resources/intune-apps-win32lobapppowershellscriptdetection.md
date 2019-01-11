---
title: Тип ресурса win32LobAppPowerShellScriptDetection
description: Содержит свойства сценария PowerShell для обнаружения приложений Win32
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bdd3c0e6864a3568b4f1efb7c1c18a25f3e7c84d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863030"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>Тип ресурса win32LobAppPowerShellScriptDetection

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства сценария PowerShell для обнаружения приложений Win32

Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enforceSignatureCheck|Логический|Значение, указывающее, применяется ли проверка подписи|
|runAs32Bit|Логический|Значение, указывающее, будет ли этот скрипт должна запускаться в 32-разрядная версия|
|scriptContent|Строка|Содержимое сценария для обнаружения Win32 строки из бизнес-приложения в кодировке base64|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```





