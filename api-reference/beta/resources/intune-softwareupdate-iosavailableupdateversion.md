---
title: Тип ресурса Иосаваилаблеупдатеверсион
description: сведения о доступных версиях обновлений iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bd229d0a8d10bb9321ea1d051294f7bde87e212
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089401"
---
# <a name="iosavailableupdateversion-resource-type"></a>Тип ресурса Иосаваилаблеупдатеверсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

сведения о доступных версиях обновлений iOS

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|productVersion|String|Версия обновления.|
|постингдатетиме|DateTimeOffset|Дата разноски обновления.|
|expirationDateTime|DateTimeOffset|Дата окончания срока действия обновления.|
|суппортеддевицес|Коллекция String|Список поддерживаемых устройств для обновления.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```






