---
title: Тип ресурса Иосаваилаблеупдатеверсион
description: сведения о доступных версиях обновлений iOS
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91fa2d9d6c770d67b185d94c91200ce6fc5b23b7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455032"
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



