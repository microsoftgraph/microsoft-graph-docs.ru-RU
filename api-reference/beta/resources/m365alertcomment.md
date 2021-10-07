---
title: тип ресурса m365AlertComment
description: Комментарий, созданный аналитиком, связанный с предупреждением или инцидентом.
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c3c59422a8e379bbe7ecf43890774a9474d51b26
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220865"
---
# <a name="m365alertcomment-resource-type"></a>тип ресурса m365AlertComment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Комментарий, созданный аналитиком, связанный с предупреждением или инцидентом. 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|comment|String|Текст комментария.|
|createdByDisplayName|String|Лицо или имя приложения, которое отправило комментарий.|
|createdDateTime|DateTimeOffset|Время отправки комментария.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.m365AlertComment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.m365AlertComment",
  "comment": "String",
  "createdByDisplayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

