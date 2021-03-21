---
title: тип ресурса riskyUser
description: Представляет пользователей Azure AD, которые находятся в опасности. Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям в Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d2e0942e92b1dcd648812503a923dac51a640be1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960329"
---
# <a name="riskyuser-resource-type"></a>тип ресурса riskyUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей Azure AD, которые находятся в опасности. Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям в Azure AD.

Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)

>**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список riskyUsers](../api/riskyusers-list.md) | [коллекция riskyUser](riskyuser.md)|Список рискованных пользователей и их свойств.|
|[Get riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|Получите определенного рискованного пользователя и его свойства.|
|[История списка](../api/riskyuser-list-history.md) | [riskyUserHistoryItem](riskyuserhistoryitem.md) collection|Получите историю рисков пользователя Azure AD.|
|[Подтверждение скомпрометации riskyUsers](../api/riskyusers-confirmcompromised.md)|Нет |Подтвердит риск пользователя как скомпрометированного.|
|[Увольнение riskyUsers](../api/riskyusers-dismiss.md)|Нет | Отклонять риск рискованного пользователя.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный ID пользователя в опасности.|
|isDeleted|boolean|Указывает, удален ли пользователь. Возможные значения: `true`, `false`.|
|isProcessing|boolean|Указывает, обрабатывается ли приложением рискованное состояние пользователя.|
|riskLastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления рискованного пользователя.  Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|riskLevel|riskLevel| Уровень обнаруженного рискованного пользователя. Возможные значения `low` , `medium` `high` , , `hidden` , `none` `unknownFutureValue` .  |
|riskState|riskState| Состояние риска пользователя. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.  |
|riskDetail|riskDetail| Возможные `none` значения: `adminGeneratedTemporaryPassword` , `userPerformedSecuredPasswordChange` , , , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` , `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` , .  |
|userDisplayName|string|Рискованное имя отображения пользователя.|
|userPrincipalName|string|Рискованное основное имя пользователя.|

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
