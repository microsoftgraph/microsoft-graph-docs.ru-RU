---
title: тип ресурса workforceIntegrationEncryption
description: Объект шифрования, определяющий протокол и секрет для интеграции рабочей силы.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a05111fb561fe806b8b590eef321e3b7fcc9ebcd9054d2d8e5f7853e6d0c88b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180455"
---
# <a name="workforceintegrationencryption-resource-type"></a>тип ресурса workforceIntegrationEncryption

Пространство имен: microsoft.graph

Объект шифрования, определяющий протокол и секрет для [рабочей силы.](../resources/workforceintegration.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|протокол|String| Возможные значения: `sharedSecret`, `unknownFutureValue`.|
|секрет|String|Шифрование общего секрета.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workforceIntegrationEncryption",
  "baseType": null
}-->

```json
{
  "protocol": "String",
  "secret": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workforceIntegrationEncryption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

