---
title: тип ресурса assignmentFilterEvaluateRequest
description: Запрос на оценку фильтра назначения для устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7a3af607c2d809f32e064b45bfaef9d6057f241f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697424"
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
|правило|String|Определение правила фильтра назначения.|
|top|Int32|Ограничение записей на запрос. Значение по умолчанию — 100, если предоставлено менее 0 или более 100|
|skip|Int32|Количество записей, которые нужно пропустить. Значение по умолчанию — 0|

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
  "skip": 1024
}
```



