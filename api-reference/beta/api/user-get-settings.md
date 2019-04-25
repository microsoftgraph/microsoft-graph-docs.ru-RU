---
title: Получение параметров
description: Чтение объекта параметров пользователя и Организации.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128feebf624350baaea9fee41c411bd46c2b42c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536577"
---
# <a name="get-settings"></a>Получение параметров

Чтение объекта [параметров](../resources/user-settings.md) пользователя и Организации.
Чтобы узнать, как обновить свойства объекта [Settings](../resources/user-settings.md) , ознакомьтесь со статьей [Обновление параметров пользователя](user-update-settings.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read.All, User.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User. Read. ALL, User. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

```http
GET /me/settings/
```

Запрос с идентификатором пользователя или userPrincipalName доступен только пользователю или пользователем с разрешениями User. ReadWrite. ALL. Чтобы узнать больше, ознакомьтесь [](/graph/permissions-reference)с разрешениями.

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [пользовательских параметров](../resources/user-settings.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

