---
title: Получение параметров
description: Чтение объекта параметры пользователей и организаций.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: ace7c43b27860832968572628838484bc8c91c84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815493"
---
# <a name="get-settings"></a>Получение параметров

Чтение объекта [Параметры](../resources/user-settings.md) пользователей и организаций.
Чтобы узнать, как обновить свойства объекта [параметров](../resources/user-settings.md) , обратитесь к разделу [Изменение параметров пользователей](user-update-settings.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read.All, User.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All,User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

```http
GET /me/settings/
```

Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All. [Для получения дополнительных сведений см.](/graph/permissions-reference)

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>Тело запроса

Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` объект [параметров пользователя](../resources/user-settings.md) и кода ответа в теле ответа.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a>Ответ

Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

