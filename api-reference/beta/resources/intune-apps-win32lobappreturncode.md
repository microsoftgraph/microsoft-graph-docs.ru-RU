---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3110ea120f88f56e49cfe33bf1b47631dc5c1f86
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422618"
---
# <a name="win32lobappreturncode-resource-type"></a>Тип ресурса win32LobAppReturnCode

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства кода возврата для приложения Win32

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ретурнкоде|Int32|Возвращаемый код.|
|type|[win32LobAppReturnCodeType](../resources/intune-apps-win32lobappreturncodetype.md)|Тип кода возврата. Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.|

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



