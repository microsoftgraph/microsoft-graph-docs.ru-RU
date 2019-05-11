---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37abd83b34fde565aa78e62454c4ce7d47ea192a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950412"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса Excludedapps к объекту

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства исключенных приложений Office365.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|обращения|Логический|Значение, если доступ к MS Office должен быть исключен или нет.|
|невозможно|Логический|Значение, заданное в поле IF MS Office Excel, не должно быть исключено.|
|тень|Логический|Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.|
|infoPath|Логический|Значение, если MS Office InfoPath следует исключить.|
|Lync|Логический|Значение, если MS Office Skype для бизнеса — не следует исключать.|
|oneDrive|Логический|Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.|
|Microsoft|Логический|Значение, если MS Office OneNote должен быть исключен или нет.|
|outlook|Логический|Значение, если MS Office Outlook следует исключить из проверки.|
|powerPoint|Логический|Значение, если MS Office PowerPoint следует исключить из проверки.|
|publisher|Логический|Значение, если MS Office Publisher должен быть исключен или нет.|
|Шарепоинтдесигнер|Логический|Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.|
|Teams|Логический|Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.|
|Visio|Логический|Значение, заданное для if MS Office Visio, должно быть исключено.|
|текстовых|Логический|Значение, заданное для if MS Office Word, должно быть исключено.|

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
  "teams": true,
  "visio": true,
  "word": true
}
```




