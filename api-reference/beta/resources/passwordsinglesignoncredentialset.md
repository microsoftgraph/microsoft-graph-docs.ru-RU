---
title: Тип ресурса Пассвордсинглесигнонкредентиалсет
description: Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 87aafa6e21171088f9b4b5eac318f6c9551e18ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998203"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a>Тип ресурса Пассвордсинглесигнонкредентиалсет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|записей|Коллекция [учетных данных](credential.md)|Список объектов учетных данных, определяющих полный вход.|
|id|String|Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet",
  "baseType": null
}-->

```json
{
  "credentials": [{"@odata.type": "microsoft.graph.credential"}],
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnCredentialSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


