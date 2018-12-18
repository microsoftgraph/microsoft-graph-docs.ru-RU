---
title: Тип ресурса managedDeviceReportedApp
description: Данные приложения для создания отчетов
author: tfitzmac
ms.openlocfilehash: 7fd01c5fd7553769653abd6e16ecc9ec40a79b8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359495"
---
# <a name="manageddevicereportedapp-resource-type"></a>Тип ресурса managedDeviceReportedApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Данные приложения для создания отчетов
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
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





