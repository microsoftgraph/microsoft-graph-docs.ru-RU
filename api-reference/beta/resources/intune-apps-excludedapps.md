---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d90954bda8a5bd6c9bfdeb6af0d2946b48215d00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553052"
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
|Teams|Логический|Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.|
|Visio|Логический|Значение, заДанное для if MS Office Visio, должно быть исключено.|
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
  "teams": true,
  "visio": true,
  "word": true
}
```





