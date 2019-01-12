---
title: Тип ресурса win32LobAppReturnCode
description: Содержит код возврата свойства для приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0728ee3c029331b37369172373ef1400dde37991
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927865"
---
# <a name="win32lobappreturncode-resource-type"></a>Тип ресурса win32LobAppReturnCode

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит код возврата свойства для приложения Win32
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|код возврата|Int32|Код возврата.|
|type|[win32LobAppReturnCodeType](../resources/intune-apps-win32lobappreturncodetype.md)|Тип возвращаемого кода. Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```





