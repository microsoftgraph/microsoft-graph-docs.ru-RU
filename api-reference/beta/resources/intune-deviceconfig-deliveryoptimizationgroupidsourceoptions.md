---
title: Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс
description: Тип параметров идентификатора группы
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 741b39245c26858d4cae46923d1078f568cf6945
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526768"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a>Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип параметров идентификатора группы


Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|граупидсаурцеоптион|[deliveryOptimizationGroupIdOptionsType](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|Установите эту политику, чтобы ограничить выбор однорангового узла определенным источником. Возможные значения: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```



