---
title: Начало работы с API методов проверки подлинности Microsoft Graph
description: API методов проверки подлинности в Microsoft Graph дает организациям возможность программно управлять методами проверки подлинности пользователей, получая пользователей, зарегистрированных для многофакторной проверки подлинности (MFA) и самостоятельного сброса пароля (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8f08ae59f7a2ad0e16c4fc0c3af5637bcbfaaca
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272813"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a>Начало работы с API методов проверки подлинности Microsoft Graph

[Методы проверки подлинности](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) — это способы проверки подлинности пользователей в Azure Active Directory (Azure AD). Методы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которые могут управляться сегодня в Microsoft Graph, среди многих других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator. Методы проверки подлинности используются в основной, второй фактор и пошаговой проверке подлинности, а также в процессе самообслуживания пароля (SSPR).

Для управления методами проверки подлинности пользователя можно использовать API метода проверки подлинности. Например, вы можете:

* Добавление номера телефона для пользователя, который может использовать этот номер для проверки подлинности SMS и голосовых вызовов, если они включены для использования политикой
* Обновление или удаление номера телефона, назначенного пользователю
* Включение и выключение номера для входа в SMS
* Сброс пароля пользователя

API — это ключевой инструмент для управления методами проверки подлинности пользователей.

В этом руководстве вы узнаете, как:

> [!div class="checklist"]
> * Проверка подлинности в Azure AD с правильными ролями и разрешениями
> * Проверка методов проверки подлинности пользователя
> * Добавление новых номеров телефонов для пользователя
> * Удаление номера телефона пользователя
> * Сброс пароля пользователя

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a>Шаг 1: проверка подлинности в Azure AD с правильными ролями и разрешениями

С помощью избранного [средства для взаимодействия с Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph)выполните вход с помощью учетной записи с одной из этих ролей:

* Глобальный администратор
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

Затем измените свои разрешения. Мы будем использовать [усераусентикатионмесод. ReadWrite. ALL](permissions-reference.md#user-authentication-method-permissions-preview) для этого руководства, поэтому убедитесь, что он включен в проводнике Graph или приложении.

Когда область будет назначена и отправлена, вы можете начать использовать API. В приведенных ниже примерах используется стандартный пользователь с именем Avery Говард. Следует использовать уже существующую тестовую учетную запись или создать новую с помощью приведенных ниже [инструкций](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user). Эти API являются реальными, поэтому их не следует тестировать на реальных пользователях.

## <a name="step-2-check-the-users-authentication-methods"></a>Шаг 2: проверка методов проверки подлинности пользователя

Выполните вызов, чтобы увидеть методы проверки подлинности пользователя. Сделайте URL-адрес, чтобы просмотреть профиль пользователя, и добавьте `/authentication/methods` :

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a>Отклик

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

## <a name="step-3-add-new-phone-numbers-for-the-user"></a>Шаг 3: Добавление новых номеров телефонов для пользователя

На предыдущем шаге для нового пользователя (Avery) записывается только пароль. Чтобы назначить новый номер телефона для использования с помощью параметра Avery, сделайте `POST` запрос с типом телефона и номером в тексте сообщения. Чтобы сообщить системе, что номер телефона добавлен, также необходимо изменить конец URL-адреса с `methods` на `phoneMethods` .

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "mobile",
    "phoneNumber": "+1 2065550123"
}
```

### <a name="response"></a>Отклик

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

Чтобы добавить номер Office для Office, `POST` повторите попытку с тем же URL-адресом, но измените тип и номер телефона:

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "office",
    "phoneNumber": "+1 4255550199"
}
```

### <a name="response"></a>Отклик

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

Сделайте еще один дополнительный `GET` URL-адрес методов телефона, чтобы просмотреть все номера телефонов Avery:

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a>Отклик

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods",
    "value": [
        {
            "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
            "phoneNumber": "+1 4255550199",
            "phoneType": "office",
            "smsSignInState": "notSupported"
        },
        {
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        }
    ]
}
```

Убедитесь, что вы видите оба числа, как ожидалось.

## <a name="step-4-remove-a-phone-number-from-the-user"></a>Шаг 4: Удаление номера телефона пользователя

В этом сценарии Avery теперь работает с домашней страницы, поэтому вам нужно удалить номер Office из своей учетной записи. Вам нужно позвонить по `DELETE` URL-адресу Office Phone, который можно создать, добавив идентификатор Office Phone в URL-адрес методов телефона. Просмотрите список номеров телефонов, приведенный в разделе Avery: номер офиса начинается с "e37f".

### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

В ответе нет данных, так как для него больше не предусмотрено Office Phone. Вы можете убедиться, что он просматривает все методы Avery, которые были `GET` сделаны ранее:

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a>Отклик

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        },
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

Как и ожидалось, теперь у пользователя есть только один мобильный телефон и пароль.

## <a name="step-5-reset-the-users-password"></a>Шаг 5: Сброс пароля пользователя

В этом сценарии Avery забыл пароль и его необходимо сбросить. Для сброса необходимо указать `POST` URL-адрес своего пароля (в списке методы проверки подлинности, начинающийся с "28c1"), с указанием действия "ресетпассворд". Введите новый пароль в теле запроса.

### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a>Отклик

```
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

Так как это приведет к синхронизации пароля в Active Directory в локальной инфраструктуре клиента, может потребоваться несколько минут, поэтому у вас есть адрес, по которому можно проверить, завершена ли работа. Этот адрес находится в заголовке местоположения ответа, и для просмотра состояния выполните `GET` по этому URL-адресу.

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a>Отклик

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('ed178e23-7447-4892-baf8-fc46f8af26ce')/authentication/operations/$entity",
    "id": "74bfa1a6-c0e0-4957-8c37-f91048f4959e",
    "createdDateTime": "2020-05-14T00:23:40Z",
    "lastActionDateTime": "2020-05-14T00:23:41Z",
    "status": "succeeded",
    "statusDetail": "ResetSuccess",
    "resourceLocation": "https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/methods/28c10230-6103-485e-b985-444c60001490"
}
```

И успешное выполнение! Вы проверили Просмотр профиля пользователя, методов проверки подлинности, добавления и удаления номеров телефонов, а также сброса пароля. Теперь вы готовы к управлению методами своих пользователей.

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для методов проверки подлинности?

* [Общие сведения об API методов проверки подлинности Azure AD](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

* Узнайте [, как использовать REST API метода проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).
* Используйте Azure AD для [аутентификации](/graph/auth) в Microsoft Graph.
* Интегрируйте [вход в Azure AD](https://azure.microsoft.com/develop/identity/signin/) в свое приложение или в свой веб-сайт.
* Сведения о новых возможностях API Azure AD см. в [журнале изменений](changelog.md).
* Изучите [примеры](https://developer.microsoft.com/graph/graph/examples), чтобы получить более четкое представление об использовании Microsoft Graph.
