---
title: Тип ресурса Пассвордсинглесигнонкредентиалсет
description: Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9191362f0e6c98d57c609445fbe1caf3bdd775a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522006"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a>Тип ресурса Пассвордсинглесигнонкредентиалсет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает набор учетных данных, которые полностью определяют последовательность входа для пользователя или группы в приложение.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|записей|Коллекция [учетных данных](credential.md)|Список объектов учетных данных, определяющих полный вход.|
|id|Строка|Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.|

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
