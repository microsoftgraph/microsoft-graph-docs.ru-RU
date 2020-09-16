---
title: Обновление teamsApp
description: 'Обновление приложения, опубликованного ранее в каталоге приложений Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0dc3c5f3021c5479ef3eb6f227d7fbe512e0c122
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843165"
---
# <a name="update-teamsapp"></a>Обновление teamsApp

Пространство имен: microsoft.graph

Обновление [приложения](../resources/teamsapp.md) , опубликованного ранее в каталоге приложений Microsoft Teams. Чтобы обновить приложение, свойству **distributionMethod** для приложения необходимо присвоить значение `organization` .

Этот API-интерфейс специально обновляет приложение, опубликованное в каталоге приложений вашей организации (Каталог приложений клиента).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Только глобальные администраторы могут вызывать этот API.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись)     | CamlQuery. ReadWrite. ALL, Directory. ReadWrite. ALL |
| Делегированные (рабочая или учебная учетная запись) | AppCatalog.Submit|
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается|
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type  | Application/ZIP. Обязательно. |

## <a name="request-body"></a>Тело запроса

В тексте запроса включите полезные данные манифеста ZIP для Teams. Дополнительные сведения см. [в статье Создание пакета приложения](/microsoftteams/platform/concepts/apps/apps-package)

>**Примечание:** Используйте идентификатор, возвращенный при вызове [списка опубликованных приложений](./teamsapp-list.md) , для ссылки на приложение, которое вы хотите обновить. Не используйте идентификатор из манифеста пакета приложения ZIP.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a>Пример 1: обновление приложения, опубликованного ранее в каталоге приложений Microsoft Teams

### <a name="request"></a>Запрос

<!-- markdownlint-disable MD034 -->
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
