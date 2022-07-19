---
title: Тип ресурса submissionDetectedFile
description: Представляет сведения об обнаруженном файле в отправке угрозы.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5d12212968b55125776831b770f93b1e482162b3
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856897"
---
# <a name="submissiondetectedfile-resource-type"></a>Тип ресурса submissionDetectedFile

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об обнаруженном файле в отправке угрозы.

## <a name="properties"></a>Свойства
| Свойство | Тип   | Описание    |
|:---------|:-------|:---------------|
| fileHash | String | Хэш файла. |
| fileName | String | Имя файла. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionDetectedFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionDetectedFile",
  "fileName": "String",
  "fileHash": "String"
}
```

