---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d90954bda8a5bd6c9bfdeb6af0d2946b48215d00
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791791"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса Excludedapps к объекту

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства исключенных приложений Office365.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|обращения|Boolean|Значение, если доступ к MS Office должен быть исключен или нет.|
|невозможно|Boolean|Значение, заДанное в поле IF MS Office Excel, не должно быть исключено.|
|тень|Boolean|Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.|
|infoPath|Boolean|Значение, если MS Office InfoPath следует исключить.|
|Lync|Boolean|Значение, если MS Office Skype для бизнеса — не следует исключать.|
|oneDrive|Boolean|Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.|
|Microsoft|Boolean|Значение, если MS Office OneNote должен быть исключен или нет.|
|outlook|Boolean|Значение, если MS Office Outlook следует исключить из проверки.|
|powerPoint|Boolean|Значение, если MS Office PowerPoint следует исключить из проверки.|
|publisher|Boolean|Значение, если MS Office Publisher должен быть исключен или нет.|
|Шарепоинтдесигнер|Boolean|Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.|
|Teams|Boolean|Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.|
|Visio|Boolean|Значение, заДанное для if MS Office Visio, должно быть исключено.|
|текстовых|Boolean|Значение, заДанное для if MS Office Word, должно быть исключено.|

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
  "teams": true,
  "visio": true,
  "word": true
}
```





