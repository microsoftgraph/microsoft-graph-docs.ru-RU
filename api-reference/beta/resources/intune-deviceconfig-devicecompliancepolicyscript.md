---
title: Тип ресурса Девицекомплианцеполицискрипт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1a87354782ff1e8b4d90eb3c6eb5c69e1332fd4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731425"
---
# <a name="devicecompliancepolicyscript-resource-type"></a>Тип ресурса Девицекомплианцеполицискрипт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|девицекомплианцескриптид|Строка|Идентификатор сценария соответствия требованиям устройства.|
|рулесконтент|Binary|JSON правил.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyScript",
  "deviceComplianceScriptId": "String",
  "rulesContent": "binary"
}
```





