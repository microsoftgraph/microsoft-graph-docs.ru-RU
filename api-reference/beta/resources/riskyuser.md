---
title: Тип ресурса riskyUsers
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003722"
---
# <a name="riskyusers-resource-type"></a>Тип ресурса riskyUsers

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.

Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

>**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyUser.md) |Список рискованных пользователей и их свойств.|
|[Получение riskyUsers](../api/riskyusers-get.md) | [riskyUsers](riskyUser.md)|Получение определенного опасного пользователя и его свойств.|
|[Подтверждение riskyUsers скомпрометированных атак](../api/riskyusers-confirmcompromised.md)|Подтвердите опасного пользователя в качестве скомпрометированного.|
|[ОтКлонить riskyUsers](../api/riskyusers-dismiss.md)|ОтКлонить риск опасного пользователя.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|`id`|`string`|Уникальный идентификатор пользователя под угрозой|
|`isDeleted`|`bool`|Указывает, удален ли пользователь. Возможные значения: `true`,`false`|
|`isGuest`|`bool`|Указывает, является ли пользователь гостямй. Возможные значения: `true`, `false`. Имеет значение true, если удостоверение пользователя находится вне клиента. Это может быть B2B или пользователь B2C с удостоверением в Azure AD, MSA или сторонним поставщиком удостоверений. False, если удостоверение пользователя находится внутри клиента в данный момент|
|`isProcessing`|`bool`|Указывает, вехсер ли опасное состояние пользователя при обработке внутренней|
|`risk`|[особой](risk.md)|Опасное состояние пользователя|
|`riskLastUpdatedDateTime`|`datetime`|Дата и время последнего обновления рискованного пользователя|
|`userDisplayName`|`string`|Опасное отображаемое имя пользователя|
|`userPrincipalName`|`string`|Рискованное имя участника пользователя|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
 "id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
