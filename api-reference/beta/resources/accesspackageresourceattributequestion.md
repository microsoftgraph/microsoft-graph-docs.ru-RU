---
title: тип ресурса accessPackageResourceAttributeQuestion
description: Ресурс, определяющий вопрос, предоставляемый конечному пользователю, для получения значения атрибута, которое будет передано в итоге системе или в утвержденную заявку.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a5731575e5368e50699b57da419b357d145f786f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61865437"
---
# <a name="accesspackageresourceattributequestion-resource-type"></a>тип ресурса accessPackageResourceAttributeQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс, определяющий вопрос, предоставляемый конечному пользователю, для получения значения атрибута, которое будет передано в итоге системе или в утвержденную заявку.

Наследует от [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|вопрос|accessPackageQuestion|Вопрос, заданный для получения значения атрибута|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeQuestion",
  "question": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```
