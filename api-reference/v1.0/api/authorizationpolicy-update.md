---
title: Обновление аусоризатионполици
description: Обновление свойств объекта Аусоризатионполици.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ccd2e5b95059ec4e3a38eadf3f62b25377eabd3
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581242"
---
# <a name="update-authorizationpolicy"></a>Обновление Аусоризатионполици

Пространство имен: microsoft.graph

Обновление свойств объекта [аусоризатионполици](../resources/authorizationpolicy.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированное (рабочая или учебная учетная запись)     | Policy.ReadWrite.Authorization|
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | Policy.ReadWrite.Authorization|

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String| Отображаемое имя для этой политики. |
|description|String| Описание этой политики.|
|блоккмсолповершелл|Логический| Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true. Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не повлияет на Azure AD Connect или Microsoft Graph. |
|defaultUserRolePermissions|[defaultUserRolePermissions](../resources/defaultuserrolepermissions.md)| Задает определенные настраиваемые разрешения для роли пользователя по умолчанию. |
|allowedToUseSSPR|Логический| Указывает, может ли функция сброса пароля Self-Serve использоваться пользователями клиента. |
|allowedToSignUpEmailBasedSubscriptions|Логический| Указывает, могут ли пользователи регистрироваться на почтовые подписки. |
|allowEmailVerifiedUsersToJoinOrganization|Логический| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. |
|алловинвитесфром|String|Указывает, кто может приглашать внешних пользователей в Организации. Возможные значения:<ul><li>`none` — Запретить всем, в том числе администраторам, приглашать внешних пользователей. Настройка по умолчанию для государственных организаций США.</li><li>`adminsAndGuestInviters` — Разрешить членам группы "Администраторы", "Администраторы пользователей" и "гость" приглашать внешних пользователей.</li><li>`adminsGuestInvitersAndAllMembers` — Разрешить внешним пользователям приглашать этих ролей администратора и других участников роли пользователей.</li><li>`everyone` — Разрешить всем пользователям в Организации, в том числе гостям, приглашать внешних пользователей. Значение по умолчанию для всех облачных сред, кроме государственных организаций США.</li></ul> |

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a>Пример 1: обновление или Настройка уровня доступа гостей для клиента

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. В этом примере уровень гостевого доступа изменяется на "ограниченный гостевой пользователь".

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
  "allowEmailVerifiedUsersToJoinOrganization":false
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-block-msol-powershell-in-tenant"></a>Пример 2: Блокировка MSOL PowerShell в клиенте

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "blockMsolPowerShell":true
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-default-user-roles-permission-to-create-applications"></a>Пример 3: отключение разрешения роли пользователя по умолчанию для создания приложений

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions":{
      "allowedToCreateApps":false
   }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-4-enable-default-user-role-to-use-self-serve-password-reset-feature"></a>Пример 4: Включение роли пользователя по умолчанию для использования функции сброса пароля Self-Serve

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "allowedToUseSSPR":true
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-disable-user-consent-to-apps-for-default-user-role"></a>Пример 5: отключение согласия пользователя для приложений для роли пользователя по умолчанию

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_disableUserConsent"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": []
   }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-6-enable-user-consent-to-apps-subject-to-app-consent-policy"></a>Пример 6: включение согласия пользователя для приложений, подчиняются политике согласия приложений

#### <a name="request"></a>Запрос

Ниже приведен пример запроса, который разрешает согласие пользователя на приложения, в соответствии со встроенной [политикой согласия приложений](/azure/active-directory/manage-apps/manage-app-consent-policies) `microsoft-user-default-low` , которая разрешает делегированные разрешения, классифицированные как низкие, для клиентских приложений из проверенных издателей или зарегистрированных в одном клиенте.

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_enableUserConsentLow"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authorizationPolicy

{
   "defaultUserRolePermissions": {
      "permissionGrantPoliciesAssigned": [
         "managePermissionGrantsForSelf.microsoft-user-default-low"
      ]
   }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationpolicy"
} -->

```http
HTTP/1.1 204 No Content
```
