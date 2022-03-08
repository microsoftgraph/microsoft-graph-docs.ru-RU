---
title: тип ресурса cloudPcBulkRemoteActionResult
description: Представляет удаленный результат удаленного действия, заданный облачным КОМПЬЮТЕРом.
author: rongting
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 46f1336ec8f8cfa53813a73ac1230767f3a2e937
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339697"
---
# <a name="cloudpcbulkremoteactionresult-resource-type"></a>тип ресурса cloudPcBulkRemoteActionResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удаленный результат удаленного действия, заданный облачным КОМПЬЮТЕРом.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|failedDeviceIds|Коллекция String|Список всех управляемых ID-устройств Intune, завершив массовое действие с ошибкой.|
|notFoundDeviceIds|Коллекция строк|Список всех управляемых ID-устройств Intune, которые не были найдены при попытке массового действия.|
|notSupportedDeviceIds|Коллекция строк|Список всех управляемых ID устройств Intune, которые были идентифицированы как неподтвердимые для массовых действий.|
|successfulDeviceIds|Коллекция String|Список всех управляемых ID-устройств Intune, успешно завершив массовое действие.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcBulkRemoteActionResult",
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ],
  "successfulDeviceIds": [
    "String"
  ]
}
```

