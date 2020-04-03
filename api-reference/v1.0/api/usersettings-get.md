---
title: Получение параметров
description: Чтение объекта settings пользователя и организации.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5c13fc7b26b7d83ceda3a9c16d5a0d801f4f49c1
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109042"
---
# <a name="get-settings"></a>Получение параметров

Пространство имен: microsoft.graph

Чтение объекта [userSettings](../resources/usersettings.md) пользователя и организации.
Сведения об обновлении свойств объекта [userSettings](../resources/usersettings.md) см. в статье [Обновление параметров пользователя](usersettings-update.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.Read.All, User.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | User.Read.All,User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

```http
GET /me/settings/
```

Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All. Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [userSettings](../resources/usersettings.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

