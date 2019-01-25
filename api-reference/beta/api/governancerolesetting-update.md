---
title: Обновление governanceRoleSetting
description: Обновление свойств governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: e5fc297690816227e1031af363ea7d4d38199e25
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509331"
---
# <a name="update-governancerolesetting"></a>Обновление governanceRoleSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств [governanceRoleSetting](../resources/governancerolesetting.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Этот интерфейс API также требуется, что источник запроса имеют по крайней мере один `Active` назначение ролей администратора (`owner` или `user access administrator`) для ресурса.

|Тип разрешения      | Разрешения              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Authorization  | Bearer {code}|
| Content-Type  | application/json|


## <a name="request-body"></a>Текст запроса
В тексте запроса задаете значения параметра [governanceRuleSettings](../resources/governancerulesetting.md) , который требуется обновить. 

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.|
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.|
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли. Это действие не поддерживается для `pimforazurerbac` сценарий в данный момент и может быть доступно в последующих сценариях.|
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые вычисляются при попытке активировать его назначения ролей.|

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика. 

### <a name="error-codes"></a>Коды ошибок
Этот интерфейс API возвращает стандартные коды ошибок HTTP. Кроме того он возвращает следующие коды ошибок.

|Код ошибки     | Сообщение об ошибке         | Сведения             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | [GovernanceRoleSetting](../resources/governancerolesetting.md) не существует в системе.
| 400 BadRequest| InvalidRoleSetting    | Недопустимые значения [governanceRuleSettings](../resources/governancerulesetting.md) , предоставляемые в тексте запроса.

## <a name="example"></a>Пример 
В этом примере обновляется параметр роли для настраиваемых ролей 3 в Wingtip Toys - производственного подписки.
##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a>Ответ
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
