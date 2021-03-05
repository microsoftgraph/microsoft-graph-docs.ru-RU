---
title: Обновление smsAuthenticationMethodConfiguration
description: Обновление свойств объекта smsAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdcddf77f2e85517b6c8d1685b4129b1e8d83f0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475631"
---
# <a name="update-smsauthenticationmethodconfiguration"></a>Обновление smsAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновим свойства объекта [smsAuthenticationMethodConfiguration,](../resources/smsauthenticationmethodconfiguration.md) который представляет политику метода проверки подлинности текстовых сообщений для клиента Azure AD.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Policy.ReadWrite.AuthenticationMethod|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Policy.ReadWrite.AuthenticationMethod|

Для делегирования сценариев администратору требуется роль глобального администратора. Дополнительные сведения см. в [роли](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса необходимо предоставить представление JSON объекта [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) со значениями полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

В следующей таблице показаны свойства, необходимые при обновлении [объекта smsAuthenticationMethodConfiguration.](../resources/smsauthenticationmethodconfiguration.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

>**Примечание:** Свойство `@odata.type` со значением `#microsoft.graph.smsAuthenticationMethodConfiguration` должно быть включено в тело.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_smsauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
Content-Type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
    "id": "Sms",
    "state": "enabled"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "713980c7-80c7-7139-c780-3971c7803971",
  "state": "String"
}
```

