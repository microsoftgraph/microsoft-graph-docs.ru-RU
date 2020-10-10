---
title: Удаление Пассвордлессмикрософтаусентикатораусентикатионмесод
description: Удаляет объект Пассвордлессмикрософтаусентикатораусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f5b91f65326fd14fe648b9a94c54a8e0db1920f
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418524"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod"></a>Удаление Пассвордлессмикрософтаусентикатораусентикатионмесод
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаляет объект метода входа без пароля пользователя для средства [проверки подлинности Майкрософт](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) .

> [!NOTE]
> Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии. Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения, действующие на себя (от большинства до минимальных привилегий)|Разрешения, действующие на других (по крайней мере для самых привилегированных)|
|:---|:---|:--|
|Делегированные (рабочая или учебная учетная запись)|Не поддерживается.|Усераусентикатионмесод. ReadWrite. ALL
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|Не поддерживается.
|Для приложений|Не поддерживается.|Не поддерживается.

Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

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
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```


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

