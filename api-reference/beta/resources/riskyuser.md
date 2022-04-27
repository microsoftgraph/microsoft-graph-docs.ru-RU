---
title: Тип ресурса riskyUser
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователей на основе различных сигналов и машинного обучения. Этот API обеспечивает программный доступ ко всем пользователям, которым в Azure AD предоставляется риск.
author: cloudhandler
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: ff09c334f4d7301b54d70fd2527b1884bb67019e
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060537"
---
# <a name="riskyuser-resource-type"></a>Тип ресурса riskyUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователей на основе различных сигналов и машинного обучения. Этот API обеспечивает программный доступ ко всем пользователям, которым в Azure AD предоставляется риск.

Дополнительные сведения о событиях риска см[. в Azure Active Directory identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Для использования API riskyUsers требуется Azure AD Premium P2 лицензии.
> 2. Доступность рискованных пользовательских данных регулируется политиками хранения [данных Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Перечисление объектов riskyUsers](../api/riskyusers-list.md) | [Коллекция riskyUser](riskyuser.md)|Вывод списка рискованных пользователей и их свойств.|
|[Получение riskyUser](../api/riskyusers-get.md) | [riskyUser](riskyuser.md)|Получение определенного пользователя с риском и его свойств.|
|[Журнал списков](../api/riskyuser-list-history.md) | [Коллекция riskyUserHistoryItem](riskyuserhistoryitem.md)|Получение журнала рисков пользователя Azure AD.|
|[Подтверждение компрометации riskyUsers](../api/riskyusers-confirmcompromised.md)|Нет |Подтвердите, что рискованный пользователь скомпрометирован.|
|[Закрытие riskyUsers](../api/riskyusers-dismiss.md)|Нет | Отклонить риск пользователя, который является рискованным.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|id|string|Уникальный идентификатор пользователя, на который есть риск.|
|isDeleted|boolean|Указывает, удален ли пользователь. Возможные значения: `true`, `false`.|
|isProcessing|boolean|Указывает, обрабатывается ли серверной частью состояние риска пользователя.|
|riskLastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления пользователя с риском.  Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|riskLevel|riskLevel| Уровень обнаруженного пользователя, который является рискованным. Возможные значения: , , , , `hidden`. `none``unknownFutureValue``high``medium``low`  |
|riskState|riskState| Состояние риска пользователя. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.  |
|riskDetail|riskDetail| Возможные значения: , , , , , `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe``userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised``unknownFutureValue``adminConfirmedUserCompromised``hidden`. `userPerformedSecuredPasswordReset``userPerformedSecuredPasswordChange``adminGeneratedTemporaryPassword``none`  |
|userDisplayName|string|Отображаемое имя пользователя, которое является рискованным.|
|userPrincipalName|string|Имя участника-пользователя с риском.|

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
