---
title: Тип ресурса cloudPcForensicStorageAccount
description: Представляет учетную запись хранения облачного компьютера для проведения экспертного анализа.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ec722361b1d6fd1944ef22d32e2dbe38a5442741
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366334"
---
# <a name="cloudpcforensicstorageaccount-resource-type"></a>Тип ресурса cloudPcForensicStorageAccount

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об учетной записи хранения, которые можно использовать для хранения моментальных снимков или моментальных снимков облачного компьютера для проведения экспертного анализа.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|storageAccountId|String|Идентификатор учетной записи хранения.|
|storageAccountName|String|Имя учетной записи хранения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "storageAccountId",
  "@odata.type": "microsoft.graph.cloudPcForensicStorageAccount",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcForensicStorageAccount",
  "storageAccountId": "String",
  "storageAccountName": "String"
}
```
