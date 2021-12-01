---
title: сложный тип singleServicePrincipal
description: Определяет главную службу в клиенте, которая будет разрешена в качестве запрашивателя, утверждения или рецензента.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aaffcafdf0cc8f33efee350e15d0797ad5cba76e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242698"
---
# <a name="singleserviceprincipal-complex-type"></a>сложный тип singleServicePrincipal

Пространство имен: microsoft.graph

Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакетов доступа. Значение указывает, что этот subjectSet определяет определенного директора службы в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или `@odata.type` `#microsoft.graph.singleServicePrincipal` рецензента. [](../resources/subjectset.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание этого директора службы.|
|servicePrincipalId|Строка|ID [службыPrincipal](serviceprincipal.md).|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.singleServicePrincipal",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.singleServicePrincipal",
  "servicePrincipalId": "String",
  "description": "String"
}
```



