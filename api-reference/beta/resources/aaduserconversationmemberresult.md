---
title: Тип ресурса aadUserConversationMemberResult
description: Ресурс для моделирования ответов массовых операций в aadUserConversationMember.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8251107c325bdbe2c5ff9e6df95a2d08277dde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663911"
---
# <a name="aaduserconversationmemberresult-resource-type"></a>Тип ресурса aadUserConversationMemberResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельный ответ для каждого члена, указанного в массовой операции, состоящей из [aadUserConversationMember(s)](aadUserConversationMember.md) в запросе.
Этот ресурс является производным от [ресурса actionResultPart.](actionresultpart.md)

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:---------------|:--------|:----------|
|userId|`String`|ИД объекта пользователя Azure AD, добавляемого в рамках массовой операции.|
|error|[publicError](publicerror.md) |Ошибка, которая произошла (если она возникла) в ходе массовой операции.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserConversationMemberResult"
}-->

```json
{
    "userId": "string",
    "error": "microsoft.graph.publicError"
}
```

## <a name="see-also"></a>См. также

- [Массовое добавление участников в команду](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


