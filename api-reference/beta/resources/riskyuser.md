---
title: Тип ресурса Рискюсер
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f97da36c0a3a4c1d20e586293ae3ef5efcd0cdc4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601078"
---
# <a name="riskyuser-resource-type"></a>Тип ресурса Рискюсер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.

Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection).

>**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список riskyUsers](../api/riskyusers-list.md) | Коллекция [рискюсер](riskyuser.md)|Список рискованных пользователей и их свойств.|
|[Получение Рискюсер](../api/riskyusers-get.md) | [рискюсер](riskyuser.md)|Получение определенного опасного пользователя и его свойств.|
|[Журнал списка](../api/riskyuser-list-history.md) | Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)|Получение журнала рисков пользователя Azure AD.|
|[Подтверждение riskyUsers скомпрометированных атак](../api/riskyusers-confirmcompromised.md)|Нет |Подтвердите опасного пользователя в качестве скомпрометированного.|
|[Отклонить riskyUsers](../api/riskyusers-dismiss.md)|Нет | Отклонить риск опасного пользователя.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|`id`|`string`|Уникальный идентификатор пользователя под угрозой.|
|`isDeleted`|`bool`|Указывает, удален ли пользователь. Возможные значения: `true`, `false`.|
|`isProcessing`|`bool`|Указывает, обрабатывается ли небезопасным состояние пользователя в серверной части.|
|`riskLastUpdatedDateTime`|`datetime`|Дата и время последнего обновления рискованного пользователя|
|`riskLevel`|`riskLevel`| Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue.  |
|`riskState`|`riskState`| Возможные значения: None, Конфирмедсафе, remediateо, Атриск, unknownFutureValue.  |
|`riskDetail`|`riskDetail`| Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, Hidden, adminConfirmedUserCompromised, unknownFutureValue.  |
|`userDisplayName`|`string`|Опасное отображаемое имя пользователя.|
|`userPrincipalName`|`string`|Опасное имя участника пользователя.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
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
