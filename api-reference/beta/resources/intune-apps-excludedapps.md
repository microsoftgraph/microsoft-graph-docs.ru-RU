---
title: тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office365.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2025df58d8ff6387fb217ec2d19e7f6d34df2499
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064569"
---
# <a name="excludedapps-resource-type"></a>тип ресурса excludedApps

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для исключенных приложений Office365.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|доступ|Boolean|Значение, если ms Office доступ должен быть исключен или нет.|
|bing|Логический|Значение, если Поиск (Майкрософт) по умолчанию, должно быть исключено или нет.|
|Excel|Boolean|Значение, если ms Office Excel следует исключить или нет.|
|groove|Boolean|Значение, если ms Office OneDrive для бизнеса - Groove, должно быть исключено или нет.|
|infoPath|Boolean|Значение, если ms Office InfoPath, должно быть исключено или нет.|
|lync|Boolean|Значение для если ms Office Skype для бизнеса - Lync следует исключить или нет.|
|oneDrive|Boolean|Значение для того, следует Office OneDrive ms или нет.|
|oneNote|Логический|Значение для того, следует Office OneNote ms или нет.|
|outlook|Boolean|Значение для того, следует Office Outlook ms или нет.|
|powerPoint|Boolean|Значение для того, следует Office PowerPoint ms или нет.|
|publisher|Boolean|Значение, если ms Office Publisher следует исключить или нет.|
|sharePointDesigner|Логический|Значение, если ms Office SharePointDesigner, должно быть исключено или нет.|
|teams|Boolean|Значение, если ms Office Teams следует исключить или нет.|
|visio|Логический|Значение, если ms Office Visio, должно быть исключено или нет.|
|слово|Логический|Значение, если ms Office Word, должно быть исключено или нет.|

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



