---
title: тип ресурса publicErrorDetail
description: Представляет сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 123655f1f75d9d05ec95d1e9e0c15815c341aa11fffb72c6f59c34bf1572bd8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138348"
---
# <a name="publicerrordetail-resource-type"></a>тип ресурса publicErrorDetail

Пространство имен: microsoft.graph

Представляет сведения о [publicError](../resources/publicerror.md) или [publicInnerError](../resources/publicinnererror.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|String|Код ошибки.|
|message|String|Сообщение об ошибке.|
|target|String|Целевое значение ошибки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```
