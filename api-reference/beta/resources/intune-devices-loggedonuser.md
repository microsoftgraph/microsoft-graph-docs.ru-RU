---
title: Тип ресурса Логжедонусер
description: Вошедший в систему пользователь
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8f1547669a2bb14c5ae84920c1eb6bef2dfbeb1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470523"
---
# <a name="loggedonuser-resource-type"></a>Тип ресурса Логжедонусер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вошедший в систему пользователь

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор пользователя|
|ластлогондатетиме|DateTimeOffset|Дата и время, когда пользователь входит в систему|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```



