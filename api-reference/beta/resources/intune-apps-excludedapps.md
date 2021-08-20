---
title: тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office365.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45051f7526ba6d7740144e42001db28eb0443c877c4363479dcdd1a476de8bd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153337"
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
|lync|Логический|Значение для если ms Office Skype для бизнеса - Lync следует исключить или нет.|
|oneDrive|Логический|Значение для того, следует Office OneDrive ms или нет.|
|oneNote|Логический|Значение для того, следует Office OneNote ms или нет.|
|outlook|Логический|Значение для того, следует Office Outlook ms или нет.|
|powerPoint|Логический|Значение для того, следует Office PowerPoint ms или нет.|
|publisher|Логический|Значение, если ms Office Publisher следует исключить или нет.|
|sharePointDesigner|Логический|Значение, если ms Office SharePointDesigner, должно быть исключено или нет.|
|teams|Логический|Значение, если ms Office Teams следует исключить или нет.|
|visio|Логический|Значение, если ms Office Visio, должно быть исключено или нет.|
|слово|Логический|Значение, если ms Office Word, должно быть исключено или нет.|

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




