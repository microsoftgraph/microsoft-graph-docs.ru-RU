---
title: Тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office 365.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90216c639d36a989b2fad5dbdc1adbd11fe46ede
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943951"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса excludedApps

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для исключенных приложений Office 365.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Access|Логический|Значение для Если MS Office Access следует исключить или нет.|
|в приложении Excel|Логический|Значение для Если MS Office Excel следует исключить или нет.|
|Groove|Логический|Значение для Если MS Office OneDrive для бизнеса - Groove следует исключить или нет.|
|infoPath|Логический|Значение для Если MS Office InfoPath следует исключить или нет.|
|Lync|Логический|Значение для Если Скайп MS Office для бизнес - Lync следует исключить или нет.|
|oneDrive|Логический|Значение для Если MS Office OneDrive следует исключить или нет.|
|oneNote|Логический|Значение для Если MS Office OneNote следует исключить или нет.|
|Outlook|Логический|Значение для Если MS Office Outlook следует исключить или нет.|
|powerPoint|Логический|Значение для Если MS Office PowerPoint следует исключить или нет.|
|publisher|Логический|Значение для Если MS Office Publisher следует исключить или нет.|
|sharePointDesigner|Логический|Значение для Если MS Office SharePointDesigner следует исключить или нет.|
|visio|Логический|Значение для Если MS Office Visio следует исключить или нет.|
|Word|Логический|Значение для Если MS Office Word следует исключить или нет.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "visio": true,
  "word": true
}
```





