---
title: непрерывный Тип ресурсовAccessEvaluationSessionControl
description: Управление сеансами для контроля параметров непрерывной оценки доступа.
author: lujiangfeng666
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: caa6c09d54d2305af348b848d99e0e43049f5c55
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450802"
---
# <a name="continuousaccessevaluationsessioncontrol-resource-type"></a>непрерывный Тип ресурсовAccessEvaluationSessionControl

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление сеансами для контроля параметров непрерывной оценки доступа.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|mode|continuousAccessEvaluationMode| Указывает параметры непрерывной оценки доступа. Допустимые значения: `strictEnforcement`, `disabled`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationSessionControl"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationSessionControl",
  "mode": "String"
}
```
