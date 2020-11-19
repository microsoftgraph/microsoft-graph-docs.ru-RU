---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6408ee1cef68ade4ccb1c8b90f91ca99a5b75bf4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230900"
---
# <a name="osversioncount-resource-type"></a>Тип ресурса Осверсионкаунт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество устройств с вредоносной программой для каждой версии ОС

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|osVersion|String|Версия ОС|
|deviceCount|Int32|Количество устройств с вредоносной программой для версии ОС|
|lastUpdateDateTime|DateTimeOffset|Метка времени последнего обновления числа устройств в формате UTC|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




