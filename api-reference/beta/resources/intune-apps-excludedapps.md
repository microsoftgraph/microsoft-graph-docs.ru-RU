---
title: Тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office 365.
author: tfitzmac
ms.openlocfilehash: b8c9eff985783c953ff099dbf4d5ba00826652c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344627"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса excludedApps

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для исключенных приложений Office 365.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Access|Boolean.|Значение для Если MS Office Access следует исключить или нет.|
|в приложении Excel|Boolean.|Значение для Если MS Office Excel следует исключить или нет.|
|Groove|Boolean.|Значение для Если MS Office OneDrive для бизнеса - Groove следует исключить или нет.|
|infoPath|Boolean.|Значение для Если MS Office InfoPath следует исключить или нет.|
|Lync|Boolean.|Значение для Если Скайп MS Office для бизнес - Lync следует исключить или нет.|
|oneDrive|Boolean.|Значение для Если MS Office OneDrive следует исключить или нет.|
|oneNote|Boolean.|Значение для Если MS Office OneNote следует исключить или нет.|
|Outlook|Boolean.|Значение для Если MS Office Outlook следует исключить или нет.|
|powerPoint|Boolean.|Значение для Если MS Office PowerPoint следует исключить или нет.|
|publisher|Boolean.|Значение для Если MS Office Publisher следует исключить или нет.|
|sharePointDesigner|Boolean.|Значение для Если MS Office SharePointDesigner следует исключить или нет.|
|visio|Boolean.|Значение для Если MS Office Visio следует исключить или нет.|
|Word|Boolean.|Значение для Если MS Office Word следует исключить или нет.|

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





