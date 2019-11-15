---
title: 'servicePrincipal: Упдатепассвордсинглесигнонкредентиалс'
description: Обновление учетных данных единого входа с помощью пароля пользователя или группы.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef480c7f40fe74a46ded87c588f4a7c4eb628d26
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658816"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a>servicePrincipal: Упдатепассвордсинглесигнонкредентиалс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление учетных данных единого входа с помощью пароля пользователя или группы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. AccessAsUser. ALL, Directory. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. ReadWrite. ALL |

> [!NOTE]
> Пользователи могут самостоятельно создавать учетные данные. Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор. Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.|
|записей|Коллекция [учетных данных](../resources/credential.md)|Список объектов учетных данных, определяющих полный вход.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_updatepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58",
  "credentials": [
    {
      "fieldId": "param_username",
      "value": "myusername",
      "type": "username"
    },
    {
      "fieldId": "param_password",
      "value": "pa$$w0rd",
      "type": "password"
    }
  ]
}
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: updatePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
