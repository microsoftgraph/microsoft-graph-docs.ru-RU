---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4a481d52b06c59d9d79df439b41152600af989
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274287"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса Excludedapps к объекту

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства исключенных приложений Office365.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|обращения|Boolean|Значение, если доступ к MS Office должен быть исключен или нет.|
|Bing|Boolean|Значение, если Microsoft Search по умолчанию следует исключить.|
|невозможно|Boolean|Значение, заданное в поле IF MS Office Excel, не должно быть исключено.|
|тень|Boolean|Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.|
|infoPath|Boolean|Значение, если MS Office InfoPath следует исключить.|
|Lync|Boolean|Значение, если MS Office Skype для бизнеса — не следует исключать.|
|oneDrive|Boolean|Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.|
|Microsoft|Boolean|Значение, если MS Office OneNote должен быть исключен или нет.|
|outlook|Boolean|Значение, если MS Office Outlook следует исключить из проверки.|
|powerPoint|Boolean|Значение, если MS Office PowerPoint следует исключить из проверки.|
|publisher|Boolean|Значение, если MS Office Publisher должен быть исключен или нет.|
|шарепоинтдесигнер|Boolean|Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.|
|Teams|Boolean|Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.|
|Visio|Boolean|Значение, заданное для if MS Office Visio, должно быть исключено.|
|текстовых|Boolean|Значение, заданное для if MS Office Word, должно быть исключено.|

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
  "bing": true,
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




