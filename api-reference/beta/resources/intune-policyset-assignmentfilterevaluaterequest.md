---
title: тип ресурса assignmentFilterEvaluateRequest
description: Запрос на оценку фильтра назначения для устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee45c31df0eb2bdd8f65eb670af4a3a83b64f0b9
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368163"
---
# <a name="assignmentfilterevaluaterequest-resource-type"></a>тип ресурса assignmentFilterEvaluateRequest

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Запрос на оценку фильтра назначения для устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|платформа|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Тип платформы устройств, на которых будет применяться фильтр назначения. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|правило|Строка|Определение правила фильтра назначения.|
|top|Int32|Ограничение записей на запрос. Значение по умолчанию — 100, если предоставлено менее 0 или более 100|
|skip|Int32|Количество записей, которые нужно пропустить. Значение по умолчанию — 0|
|orderBy|Коллекция строк|Заказать сортировку устройств. Значение по умолчанию возрастает по имени устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluateRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluateRequest",
  "platform": "String",
  "rule": "String",
  "top": 1024,
  "skip": 1024,
  "orderBy": [
    "String"
  ]
}
```




