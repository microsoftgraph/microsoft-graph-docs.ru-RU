---
title: Обновление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Обновление свойств объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8536e70f264775a073830aeac77d3fc27810e5f0
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418494"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a>Обновление Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите свойства объекта [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , который представляет политику метода проверки подлинности входа с помощью пароля Microsoft Authenticator для клиента Azure AD.

> [!NOTE]
> Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии. Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy. ReadWrite. AuthenticationMethod|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

Для делегированных сценариев администратору требуется одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Глобальный администратор
* Глобальный читатель
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) в формате JSON со значениями полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

Список свойств приведен в разделе [пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).

>**Примечание:** `@odata.type` Свойство со значением `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` должно быть включено в текст сообщения.


## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    "state": "enabled"
}
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

