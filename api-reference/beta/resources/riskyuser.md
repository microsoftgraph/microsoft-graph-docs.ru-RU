---
title: Тип ресурса Рискюсер
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179a6cbddf3e4b27c47761bd81aad1052ae7f728
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343537"
---
# <a name="riskyuser-resource-type"></a>Тип ресурса Рискюсер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.

Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

>**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список riskyUsers](../api/riskyusers-list.md) | Коллекция [рискюсер](riskyUser.md)|Список рискованных пользователей и их свойств.|
|[Получение Рискюсер](../api/riskyusers-get.md) | [Рискюсер](riskyUser.md)|Получение определенного опасного пользователя и его свойств.|
|[Подтверждение riskyUsers скомпрометированных атак](../api/riskyusers-confirmcompromised.md)|Нет |Подтвердите опасного пользователя в качестве скомпрометированного.|
|[ОтКлонить riskyUsers](../api/riskyusers-dismiss.md)|Нет | ОтКлонить риск опасного пользователя.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|`id`|`string`|Уникальный идентификатор пользователя под угрозой|
|`isDeleted`|`bool`|Указывает, удален ли пользователь. Возможные значения: `true`,`false`|
|`isGuest`|`bool`|Указывает, является ли пользователь гостямй. Возможные значения: `true`, `false`. Имеет значение true, если удостоверение пользователя находится вне клиента. Это может быть B2B или пользователь B2C с удостоверением в Azure AD, MSA или сторонним поставщиком удостоверений. False, если удостоверение пользователя находится внутри клиента в данный момент|
|`isProcessing`|`bool`|Указывает, вехсер ли опасное состояние пользователя при обработке внутренней|
|`riskLastUpdatedDateTime`|`datetime`|Дата и время последнего обновления рискованного пользователя|
|`riskLevel`|`riskLevel`| Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue.  |
|`riskState`|`riskState`| Возможные значения: None, Конфирмедсафе, remediateо, Атриск, unknownFutureValue.  |
|`riskDetail`|`riskDetail`| Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.  |
|`userDisplayName`|`string`|Опасное отображаемое имя пользователя|
|`userPrincipalName`|`string`|Рискованное имя участника пользователя|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|лист|Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)| |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

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
"isGuest": "boolean",
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
