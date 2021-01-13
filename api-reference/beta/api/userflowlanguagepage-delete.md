---
title: Удаление userFlowLanguagePage
description: Удаляет значения в объекте userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 041151af6dfe03728578bfc42b47bbfe5c422c5f
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844914"
---
# <a name="delete-userflowlanguagepage"></a>Удаление userFlowLanguagePage

Пространство имен: microsoft.graph

Удаляет значения в [объекте userFlowLanguagePage.](../resources/userflowlanguagepage.md) Можно удалить только значения в overridesPage, который используется для настройки значений, показанных пользователю во время пользовательского пути, определенного пользовательским потоком.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityUserFlow.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|IdentityUserFlow.ReadWrite.All|

Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:

* Глобальный администратор
* Администратор потока пользователей внешнего удостоверения

## <a name="http-request"></a>HTTP-запрос

Для ссылки на содержимое в объекте необходимо использовать `$value` . Это возвращает содержимое в объекте и позволяет ссылаться на него напрямую.

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/$value
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguagepage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguagepage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguagepage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguagepage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
