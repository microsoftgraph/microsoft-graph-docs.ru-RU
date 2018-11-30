---
title: Тип ресурса managedDeviceReportedApp
description: Данные приложения для создания отчетов
ms.openlocfilehash: 820269422891e01352a7f605d62147a84facea67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075643"
---
# <a name="manageddevicereportedapp-resource-type"></a>Тип ресурса managedDeviceReportedApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Данные приложения для создания отчетов
## <a name="properties"></a>Свойства
|Свойство|Тип|Description|
|:---|:---|:---|
|appId|String|Идентификатор приложения или его пакета|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```





