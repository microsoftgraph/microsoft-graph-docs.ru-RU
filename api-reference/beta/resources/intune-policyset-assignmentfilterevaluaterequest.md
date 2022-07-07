---
title: Тип ресурса assignmentFilterEvaluateRequest
description: Запрос на оценку фильтра назначения для устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a3dde68384dcf9813167544a8d2b56c8db7a98e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666860"
---
# <a name="assignmentfilterevaluaterequest-resource-type"></a>Тип ресурса assignmentFilterEvaluateRequest

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Запрос на оценку фильтра назначения для устройств.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|платформа|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Тип платформы устройств, на которых будет применяться фильтр назначения. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|Правило|String|Определение правила фильтра назначения.|
|top|Int32|Ограничение записей на запрос. Значение по умолчанию — 100, если указано меньше 0 или больше 100|
|skip|Int32|Количество записей, которые нужно пропустить. Значение по умолчанию — 0|
|Orderby|Коллекция объектов string|Упорядочивания устройств должны быть отсортированы. Значение по умолчанию — по возрастанию по имени устройства.|
|search|String|Ключевое слово поиска, примененное к найденным устройствам области.|

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
  ],
  "search": "String"
}
```




