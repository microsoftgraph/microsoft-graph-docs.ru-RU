---
title: Обновление Говернанцеролесеттинг
description: Обновление свойств объекта Говернанцеролесеттинг.
localization_priority: Normal
ms.openlocfilehash: 73a6d8ea95d4f691cef9fc3610f7e997e9fb5be8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263520"
---
# <a name="update-governancerolesetting"></a>Обновление Говернанцеролесеттинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Этот API также требует, чтобы у автора запроса было по `Active` крайней мере одно`owner` назначение `user access administrator`роли администратора (или) для ресурса.

|Тип разрешения      | Разрешения              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Привилежедакцесс. ReadWrite. Азурересаурцес  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {code}|
| Content-Type  | application/json|


## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для [говернанцерулесеттингс](../resources/governancerulesetting.md) , которые необходимо обновить. 

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Админелигиблесеттингс|Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.|
|Админмемберсеттингс|Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.|
|Усерелигиблесеттингс|Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли. В настоящее время этот `pimforazurerbac` сценарий не поддерживается и может быть доступен в следующих сценариях.|
|Усермемберсеттингс|Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)|Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.|

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 NoContent`. Метод не возвращает данные в теле отклика. 

### <a name="error-codes"></a>Коды ошибок
Этот API возвращает стандартные коды ошибок HTTP. Кроме того, возвращаются следующие коды настраиваемых ошибок.

|Код ошибки     | Сообщение об ошибке         | Сведения             |
|:--------------| :---------------------|:--------------------|
| 400 Бадрекуест| Ролесеттингнотфаунд   | [Говернанцеролесеттинг](../resources/governancerolesetting.md) не существует в системе.
| 400 Бадрекуест| Инвалидролесеттинг    | В тексте запроса указаны недопустимые значения [говернанцерулесеттингс](../resources/governancerulesetting.md) .

## <a name="example"></a>Пример 
В этом примере обновляется параметр Role для настраиваемой роли 3 в подписке Wingtip Toys — произ.
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
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_governancerolesetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
