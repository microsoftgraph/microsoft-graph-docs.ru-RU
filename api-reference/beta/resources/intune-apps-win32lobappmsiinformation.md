---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e43b3dc9e46ed193b7547a7ce85863253445d30c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846517"
---
# <a name="win32lobappmsiinformation-resource-type"></a>Тип ресурса win32LobAppMsiInformation

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства приложения MSI для приложения Win32.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|productCode|String|Код продукта MSI.|
|productVersion|String|Версия продукта MSI.|
|upgradeCode|Строка|Код обновления MSI.|
|requiresReboot|Логический|Требуется ли приложение MSI для завершения установки перезагрузить компьютер.|
|Тип корпуса|[win32LobAppMsiPackageType](../resources/intune-apps-win32lobappmsipackagetype.md)|Тип пакета MSI. Возможные значения: `perMachine`, `perUser`, `dualPurpose`.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```





