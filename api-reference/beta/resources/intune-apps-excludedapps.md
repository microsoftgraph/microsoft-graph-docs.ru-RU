---
title: тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office365.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ac91ac42018c5fc687a0b89d7496c1fdc15c97d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783598"
---
# <a name="excludedapps-resource-type"></a>тип ресурса excludedApps

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для исключенных приложений Office365.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|доступ|Логический|Значение, если ms Office доступ должен быть исключен или нет.|
|bing|Логический|Значение, если Поиск (Майкрософт) по умолчанию, должно быть исключено или нет.|
|Excel|Логический|Значение, если ms Office Excel следует исключить или нет.|
|groove|Логический|Значение, если ms Office OneDrive для бизнеса - Groove, должно быть исключено или нет.|
|infoPath|Логический|Значение, если ms Office InfoPath, должно быть исключено или нет.|
|lync|Boolean|Значение для если ms Office Skype для бизнеса - Lync следует исключить или нет.|
|oneDrive|Boolean|Значение для того, следует Office OneDrive ms или нет.|
|oneNote|Логический|Значение для того, следует Office OneNote ms или нет.|
|outlook|Boolean|Значение для того, следует Office Outlook ms или нет.|
|powerPoint|Логический|Значение для того, следует Office PowerPoint ms или нет.|
|publisher|Boolean|Значение, если ms Office Publisher следует исключить или нет.|
|sharePointDesigner|Логический|Значение, если ms Office SharePointDesigner, должно быть исключено или нет.|
|teams|Boolean|Значение, если ms Office Teams следует исключить или нет.|
|visio|Логический|Значение, если ms Office Visio, должно быть исключено или нет.|
|слово|Boolean|Значение, если ms Office Word, должно быть исключено или нет.|

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



