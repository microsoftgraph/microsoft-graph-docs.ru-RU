---
title: Тип ресурса managedDeviceCleanupSettings
description: Определение правила, когда администратор хочет устройств, чтобы очистить.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 755fc90b957427c4b9f8ee9007decea320141601
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808976"
---
# <a name="manageddevicecleanupsettings-resource-type"></a>Тип ресурса managedDeviceCleanupSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение правила, когда администратор хочет устройств, чтобы очистить.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceInactivityBeforeRetirementInDays|Строка|Количество дней, когда устройство имеет не связаться с Intune.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```





