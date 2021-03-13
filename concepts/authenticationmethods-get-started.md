---
title: Начало работы с API способов проверки подлинности в Microsoft Graph
description: AP способов проверки подлинности в Microsoft Graph с помощью программных средств позволяет организациям управлять способами проверки подлинности пользователей, регистрировать пользователей для выполнения многофакторной проверки подлинности (MFA) и выполнять самостоятельный сброс пароля (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36385345141daa8dc782b64fa154ef97c46b3091
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761453"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a>Начало работы с API способов проверки подлинности в Microsoft Graph

[Способы проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это способы, с помощью которых происходит проверка подлинности пользователей в Azure Active Directory (Azure AD). Способы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которыми можно управлять в Microsoft Graph уже сегодня, и множество других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator. Способы проверки подлинности используются в ходе основной, двухфакторной проверки подлинности, проверки подлинности повышенного уровня, а также в процессе самостоятельного сброса пароля (SSPR).

Вы можете использовать API способа проверки подлинности для управления способами проверки подлинности пользователя. Например, вы можете:

* добавить номер телефона пользователя, который затем он может использовать для проверки подлинности с помощью SMS и голосового вызова, если применение такого способа разрешено политикой;
* обновить или удалить номер телефона, назначенный пользователю;
* включить или отключить номер для входа с помощью SMS;
* сбросить пароль пользователя.

API — это основной инструмент для управления способами проверки подлинности пользователей.

С помощью данного руководства вы научитесь:

> [!div class="checklist"]
> * выполнять проверку подлинности в Azure AD с правильными ролями и разрешениями;
> * проверять способы проверки подлинности пользователя;
> * добавлять новые номера телефонов пользователю;
> * удалять номера телефона у пользователя;
> * сбрасывать пароль пользователя.

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a>Этап 1: проверка подлинности в Azure AD с правильными ролями и разрешениями

С помощью любимого[инструмента взаимодействия с Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph) выполните вход, используя учетную запись с одной из этих ролей:

* глобальный администратор;
* привилегированный администратор проверки подлинности;
* администратор проверки подлинности.

Теперь можно изменить разрешения. В этом руководстве мы будем использовать метод [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview), поэтому убедитесь, что он включен в песочнице Graph или в приложении.

После назначения и предоставления области можно приступить к работе с API. Здесь в примерах используется стандартный пользователь с именем Андрей Говоров. Необходимо использовать уже имеющуюся тестовую учетную запись или создать новую, соблюдая [эти инструкции](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user). Это интерактивные API, поэтому не проверяйте их на реальных пользователях.

## <a name="step-2-check-the-users-authentication-methods"></a>Этап 2: проверка способов проверки подлинности пользователя

Сделайте вызов для отображения способов проверки подлинности пользователя Введите URL-адрес, чтобы просмотреть профиль пользователя, и добавьте `/authentication/methods`:

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

## <a name="step-3-add-new-phone-numbers-for-the-user"></a>Этап 3: добавление новых номеров телефонов пользователю

На предыдущем этапе новый пользователь (Андрей) зарегистрировал только пароль. Чтобы назначить новый номер телефона, который будет использовать Андрей, выполните запрос `POST` с типом телефона и номером в теле. Чтобы сообщить системе о том, что номер телефона добавлен, вам также потребуется изменить окончание URL-адреса с `methods` на `phoneMethods`.

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

Чтобы добавить рабочий номер телефона Андрея, вам потребуется выполнить запрос `POST` повторно на этот же URL-адрес, но обновить тип и номер телефона.

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

Выполните еще один запрос `GET` на URL-адрес способов проверки с помощью телефона для отображения всех номеров телефона Андрея:

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

Убедитесь, что вы видите оба номера, как и предполагалось.

## <a name="step-4-remove-a-phone-number-from-the-user"></a>Этап 4: удаление номера телефона у пользователя

В этом случае Андрей теперь работает из дома, поэтому вам нужно удалить рабочий номер из его учетной записи. Необходимо выполнить запрос `DELETE` на URL-адрес рабочего телефона, который можно создать, добавив идентификатор рабочего номера в URL-адрес способов проверки по телефону. Просмотрите список номеров телефона Андрея: идентификатор рабочего номера телефона начинается с "e37f".

### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

В отклике нет данных, так как в нем больше нет рабочего номера. Чтобы убедиться в том, что номер был удален, просмотрите все способы для Андрея. Процедура `GET` аналогична той, которая была сделана ранее.

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

Как и предполагалось, пользователь снова сможет использовать только один номер мобильного телефона и пароль.

## <a name="step-5-reset-the-users-password"></a>Этап 5: сброс пароля пользователя

В этом сценарии Андрей забыл свой пароль и вам необходимо выполнить сброс его пароля. Для сброса необходимо выполнить запрос `POST` на URL-адрес пароля (см. идентификатор, начинающийся с "28c1" выше в списке способов проверки подлинности Андрей), указав действие "resetPassword". В теле запроса укажите новый пароль.

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

``` http
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

Поскольку происходит синхронизация пароля с Active Directory в локальной инфраструктуре клиента, то этот процесс может занять несколько минут, поэтому у вас есть адрес, по которому можно проверить завершение процесса синхронизации. Этот адрес находится в заголовке расположения отклика, а для просмотра статуса выполните запрос `GET` по этому URL-адресу.

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

Выполнено! Вы ознакомились с информацией о просмотре профиля пользователя, методах проверки подлинности, добавлении и удалении номеров телефонов, а также о сбросе пароля. Теперь вы можете приступать к управлению способами для своих пользователей.

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для способов проверки подлинности?

* См. статью [Обзор API способов проверки подлинности для Azure AD](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Дальнейшие действия

* Узнайте, как [использовать API REST для способов проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).
* Используйте Azure AD для [аутентификации](./auth/index.yml) в Microsoft Graph.
* Интегрируйте [вход в Azure AD](https://azure.microsoft.com/develop/identity/signin/) в свое приложение или в свой веб-сайт.
* Сведения о новых возможностях API Azure AD см. в [журнале изменений](changelog.md).
* Изучите [примеры](https://developer.microsoft.com/graph/graph/examples), чтобы получить более четкое представление об использовании Microsoft Graph.