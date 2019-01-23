---
title: Тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office 365.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395680"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса excludedApps

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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

## <a name="relationships"></a>Отношения
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




