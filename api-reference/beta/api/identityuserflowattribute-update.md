---
title: Обновление identityUserFlowAttribute
description: Обновление свойств identityUserFlowAttribute.
ms.localizationpriority: medium
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 16a4181a33c9934adfab7e3a0612bc3c058f1b59
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974914"
---
# <a name="update-identityuserflowattribute"></a>Обновление identityUserFlowAttribute

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [identityUserFlowAttribute.](../resources/identityuserflowattribute.md) Можно обновить только настраиваемые атрибуты потока пользователей.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityUserFlow.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений| IdentityUserFlow.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор атрибутов внешних Flow удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса предопределять объект JSON одним или более свойствами, которые необходимо обновить для [объекта identityUserFlowAttribute.](../resources/identityuserflowattribute.md)

>**Примечание:** Только свойство **описания** может быть обновлено.

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|description|Строка|Описание атрибута потока пользователей. Он отображается пользователю во время регистрации.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-userflowattributes-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
