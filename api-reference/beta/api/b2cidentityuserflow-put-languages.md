---
title: Создание языков
description: Создайте пользовательский язык в пользовательском потоке Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1edc89a4de37805bc150e2d0fc9f0a2c74b262da
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843929"
---
# <a name="create-languages"></a>Создание языков

Пространство имен: microsoft.graph

Этот метод используется для создания или обновления пользовательского языка в пользовательском потоке Azure AD B2C.

**Примечание.** Перед созданием настраиваемого языка необходимо включить настройку языка в пользовательском потоке Azure AD B2C. Дополнительные сведения [см. в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)

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

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса предоставляем представление объекта [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в JSON.

В следующей таблице показаны свойства, которые можно предоставлять при создании [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор языка. Это поле является тегом языка, совместимым с [RFC 5646,](https://tools.ietf.org/html/rfc5646) и должно быть документированным ИД языка. Если он указан в теле запроса, он должен соответствовать отступу, предоставленного в URL-адресе запроса.|
|isEnabled|Boolean|Указывает, включен ли язык в пользовательском потоке. Если это не предоставлено в запросе, для isEnabled будет установлено "true".|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и объект `201 Created` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a>Пример 1. Создание настраиваемого языка в пользовательском потоке B2C Azure AD

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "id": "es-ES",
  "isEnabled": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages/$entity",
  "id": "es-ES",
  "isEnabled": true,
  "displayName": "Spanish (Spain)"
}
```

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a>Пример 2. Обновление настраиваемого языка в пользовательском потоке B2C Azure AD

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "isEnabled": false
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
