---
author: nilakhan
description: Представляет сведения для отправки документов для печати
title: тип ресурса printDocumentUploadProperties
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: df563026b92905b075c1b26a9f22929bfe7dd6afca99963306dffc24b12982a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149746"
---
# <a name="printdocumentuploadproperties-resource-type"></a>тип ресурса printDocumentUploadProperties

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Описание загружаемой документации

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentType|String|Тип контента документа (MIME).|
|documentName|String|Имя документа.|
|size|Int64|Размер документа в bytes.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printDocumentUploadProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocumentUploadProperties",
  "contentType": "String",
  "documentName": "String",
  "size": "Integer"
}
```

