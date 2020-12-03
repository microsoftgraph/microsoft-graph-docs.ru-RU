---
title: Получить установленное приложение для пользователя
description: Получение приложения, установленного в личной области указанного пользователя.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 746526837761eaa04e86b33bd92792ef7e859d61
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564078"
---
# <a name="get-installed-app-for-user"></a>Получить установленное приложение для пользователя

Пространство имен: microsoft.graph

Получение [приложения](../resources/teamsappinstallation.md) , установленного в личной области указанного [пользователя](../resources/user.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | Теамсаппинсталлатион. Реадфорусер, Теамсаппинсталлатион. Read, Теамсаппинсталлатион. Реадвритеселффорусер, TeamsAppInstallation. ReadWriteForUser, TeamsAppInstallation. ReadWrite |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Теамсаппинсталлатион. Реадфорусер. ALL, Теамсаппинсталлатион. Read. ALL, Теамсаппинсталлатион. Реадвритеселффорусер. ALL, TeamsAppInstallation. ReadWriteForUser. ALL, TeamsAppInstallation. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и [приложение](../resources/teamsappinstallation.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-an-app-installed-for-the-specified-user"></a>Пример 1: получение приложения, установленного для указанного пользователя

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-the-app-installed-for-the-user"></a>Пример 2: получение имен и других сведений о приложении, установленном для пользователя

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
} -->

```http
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=?$expand=teamsAppDefinition
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
          "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('5b649834-7412-4cce-9e69-176e95a394f5')/installedApps(teamsAppDefinition())/$entity",
          "id": "NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=",
          "teamsAppDefinition": {
                                  "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk=",
                                  "teamsAppId": "a6b63365-31a4-4f43-92ec-710b71557af9",
                                  "displayName": "Power Apps",
                                  "version": "0.9"
                                }
          }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User get teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
