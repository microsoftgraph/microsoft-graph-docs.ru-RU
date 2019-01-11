---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4b7983d20f22be5f8cce24a5c362926d00de55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851599"
---
# <a name="vpplicensingtype-resource-type"></a>Тип ресурса vppLicensingType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|supportUserLicensing|Boolean|Указывает, поддерживает ли программа тип лицензирования пользователя.|
|supportDeviceLicensing|Boolean|Указывает, поддерживает ли программа тип лицензирования устройства.|
|supportsUserLicensing|Boolean|Указывает, поддерживает ли программа тип лицензирования пользователя.|
|supportsDeviceLicensing|Boolean|Указывает, поддерживает ли программа тип лицензирования устройства.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





