---
title: Обновление userFlowLanguagePage
description: Обновление значений в объекте userFlowLanguagePage.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 61a78b63099294a030daa677179b855e1a81d67d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013284"
---
# <a name="update-userflowlanguagepage"></a>Обновление userFlowLanguagePage

Пространство имен: microsoft.graph

Обновление значений в объекте userFlowLanguagePage. Вы можете обновлять значения только в переопределяемой странице, которая используется для настройки значений, показанных пользователю во время пользовательского пути, определенного потоком пользователей.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityUserFlow.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|IdentityUserFlow.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор внешних Flow удостоверений

## <a name="http-request"></a>HTTP-запрос

Чтобы ссылаться на содержимое объекта, необходимо использовать `$value` . Это возвращает содержимое объекта и позволяет ссылаться на него напрямую.

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
PUT /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON для значений, содержащихся в [пользовательском интерфейсеFlowLanguagePage.](../resources/userflowlanguagepage.md)

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_overridespages"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
Content-Type: application/json

{
  "LocalizedStrings": [
        {
            "ElementType": "UxElement",
            "ElementId": null,
            "StringId": "alert_message",
            "Override": true,
            "Value": "Are you sure that you want to cancel your selection?"
        }
    ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-overridespages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-overridespages-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
