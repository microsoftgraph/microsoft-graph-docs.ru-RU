---
title: тип ресурса workforceIntegrationEncryption
description: Объект шифрования, определяющий протокол и секрет для интеграции рабочей силы.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2400a85e4177c6890424ff57e3619d86feb455c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139389"
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

