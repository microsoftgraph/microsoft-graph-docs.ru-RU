---
author: nilakhan
description: Представляет сведения для отправки документов для печати
title: тип ресурса printDocumentUploadProperties
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: 855f9fc66d7dc35c7fddc0904e76788e280fcdba
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945000"
---
# <a name="printdocumentuploadproperties-resource-type"></a>тип ресурса printDocumentUploadProperties

Пространство имен: microsoft.graph

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

