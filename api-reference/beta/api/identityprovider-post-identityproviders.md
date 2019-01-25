---
title: Создание identityProvider
description: Создайте новый identityProvider, указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.
localization_priority: Normal
ms.openlocfilehash: c0b005d729510fa68d9edd8bfea7b85687543cf2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514651"
---
# <a name="create-identityprovider"></a>Создание identityProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [identityProvider](../resources/identityprovider.md) , указав отображаемое имя, тип identityProvider, идентификатор клиента и секрет клиента.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|Не поддерживается.|

Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса для представления JSON объекта [identityProvider](../resources/identityprovider.md) . Требуются все свойства, перечисленные в следующей таблице.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения. Это идентификатор клиента, полученные при регистрации приложения с поставщиком удостоверений.|
|client_secret|String|Секрет клиента для приложения. Это секрет клиента, полученные при регистрации приложения с поставщиком удостоверений.|
|name|String|Отображаемое имя поставщика удостоверений.|
|type|String|Тип поставщика удостоверений. Оно должно быть одно из следующих значений: <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `201 Created` объект [identityProvider](../resources/identityprovider.md) и кода ответа в теле ответа. В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.

## <a name="example"></a>Пример

В следующем примере создается **identityProvider**.

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
