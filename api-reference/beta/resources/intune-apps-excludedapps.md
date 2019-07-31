---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6bd731107571e8959418466541e2947d40d16072
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006012"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса Excludedapps к объекту

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства исключенных приложений Office365.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|обращения|Boolean|Значение, если доступ к MS Office должен быть исключен или нет.|
|невозможно|Boolean|Значение, заданное в поле IF MS Office Excel, не должно быть исключено.|
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
|Visio|Boolean|Значение, заданное для if MS Office Visio, должно быть исключено.|
|текстовых|Boolean|Значение, заданное для if MS Office Word, должно быть исключено.|

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





