---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ba3e53a26ff71dde2d5a95fde811e42ba2ccb99
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154028"
---
# <a name="excludedapps-resource-type"></a>Тип ресурса Excludedapps к объекту

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства исключенных приложений Office365.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|обращения|Логический|Значение, если доступ к MS Office должен быть исключен или нет.|
|невозможно|Логический|Значение, заДанное в поле IF MS Office Excel, не должно быть исключено.|
|тень|Логический|Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.|
|infoPath|Логический|Значение, если MS Office InfoPath следует исключить.|
|Lync|Логический|Значение, если MS Office Skype для бизнеса — не следует исключать.|
|oneDrive|Логический|Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.|
|Microsoft|Логический|Значение, если MS Office OneNote должен быть исключен или нет.|
|outlook|Логический|Значение, если MS Office Outlook следует исключить из проверки.|
|powerPoint|Логический|Значение, если MS Office PowerPoint следует исключить из проверки.|
|publisher|Логический|Значение, если MS Office Publisher должен быть исключен или нет.|
|Шарепоинтдесигнер|Логический|Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.|
|visio|Логический|Значение, заДанное для if MS Office Visio, должно быть исключено.|
|текстовых|Логический|Значение, заДанное для if MS Office Word, должно быть исключено.|

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




