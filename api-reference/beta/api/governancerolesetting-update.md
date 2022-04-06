---
title: Обновление governanceRoleSetting
description: Обновление свойств governanceRoleSetting.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: governance
author: japere
ms.openlocfilehash: 5638532dd97fec4e19cfb19d1b1bf3f19c481f19
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510452"
---
# <a name="update-governancerolesetting"></a>Обновление governanceRoleSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Обновление свойств [governanceRoleSetting](../resources/governancerolesetting.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).

>**Примечание:** Этот API также требует, `Active` чтобы у запрашиваемой стороны было по крайней мере одно назначение роли администратора (`owner` или `user access administrator`) на ресурсе.

|Тип разрешения      | Разрешения              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |
### <a name="azure-resources"></a>Ресурсы Azure

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

### <a name="azure-ad"></a>Azure AD

| Тип разрешения | Разрешения |
|:--------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureAD |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

### <a name="groups"></a>Группы

|Тип разрешения | Разрешения |
|:-------------- |:----------- |
| Делегированное (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureADGroup |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {token}|
| Content-Type  | application/json|


## <a name="request-body"></a>Текст запроса
В теле запроса укажи значения [для governanceRuleSettings](../resources/governancerulesetting.md) , которые необходимо обновить. 

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|adminEligibleSettings|[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при добавлении администратором назначения подходящих ролей.|
|adminMemberSettings|[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда администратор пытается добавить назначение ролей прямого участника.|
|userEligibleSettings|[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, оцениваемые при добавлении права на назначение ролей. |
|userMemberSettings|[коллекция governanceRuleSetting](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при попытках пользователя активировать назначение ролей.|

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика. 

### <a name="error-codes"></a>Коды ошибок
Этот API возвращает стандартные коды ошибок HTTP. Кроме того, он возвращает следующие пользовательские коды ошибок.

|Код ошибки     | Сообщение об ошибке         | Details             |
|:--------------| :---------------------|:--------------------|
| 400 BadRequest| RoleSettingNotFound   | В [системе не существует системы governanceRoleSetting](../resources/governancerolesetting.md) .
| 400 BadRequest| InvalidRoleSetting    | Значения [governanceRuleSettings](../resources/governancerulesetting.md) , предоставляемые в теле запроса, не допустимы.

## <a name="example"></a>Пример 
В этом примере обновляется параметр роли для настраиваемой роли 3 в подписке Wingtip Toys - Prod.
##### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-governancerolesetting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-governancerolesetting-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response"
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
  ]
}
-->


