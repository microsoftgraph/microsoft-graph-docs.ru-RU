---
title: Обновление teamsApp
description: 'Обновление приложения, ранее опубликованного в каталоге приложений Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ca0bb22bf8be1898c376807a5df2e727f282b30d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472015"
---
# <a name="update-teamsapp"></a>Обновление teamsApp

Пространство имен: microsoft.graph

Обновление [приложения,](../resources/teamsapp.md) ранее опубликованного в каталоге приложений Microsoft Teams. Чтобы обновить приложение, необходимо задать свойство **distributionMethod** для `organization` приложения.

Этот API специально обновляет приложение, опубликованное в каталоге приложений организации (каталоге приложений клиента).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Только глобальные администраторы могут вызывать этот API.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись)     | AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается|
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a>Параметры запроса

|Свойство|Тип|Описание|
|----|----|----|
|requiresReview| Логический | Этот необязательный параметр запроса запускает процесс проверки приложения. Пользователи с привилегиями администратора могут отправлять приложения без запуска проверки. Если пользователи хотят запросить отзыв перед публикацией, они должны `requiresReview` задать . `true` Пользователь, у которого есть привилегии администратора, может не устанавливать и не устанавливать значение, и приложение будет считаться утвержденным и будет `requiresReview` `false`  публиковаться мгновенно.|

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение           |
|:--------------|:--------------  |
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type  | application/zip. Обязательно. |

## <a name="request-body"></a>Текст запроса

В теле запроса включите полезной нагрузкой манифест Teams zip. Дополнительные сведения см. [в материале Create an app package](/microsoftteams/platform/concepts/apps/apps-package)

>**Примечание:** Используйте ID, возвращенный из вызова опубликованных приложений [Списка,](./appcatalogs-list-teamsapps.md) для ссылки на приложение, которое необходимо обновить. Не используйте ID из манифеста пакета почтовых приложений.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a>Пример 1. Обновление приложения, ранее опубликованного в каталоге приложений Microsoft Teams

#### <a name="request"></a>Запрос

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Дополнительные сведения о почтовом файле приложения Teams см. в [материале Create app package.](/microsoftteams/platform/concepts/apps/apps-package)
<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a>Пример 2. Обновление новой версии существующего приложения для проверки администратора до публикации в текущем каталоге клиента

#### <a name="request"></a>Запрос

<!-- markdownlint-disable MD034 -->

<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и пару `201 Created` ключей и значений: `publishingState` в `submitted` тексте ответа. *См.* [раздел TeamsAppdefinition](../resources/teamsappdefinition.md).

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appDefinition",
    "@odata.etag": "158749010",
    "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
    "teamsAppId": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
    "displayName": "Test app",
    "version": "1.0.11",
    "azureADAppId": "a651cc7d-ec54-4fb2-9d0e-2c58dc830b0b",
    "requiredResourceSpecificApplicationPermissions":[
         "ChannelMessage.Read.Group",
         "Channel.Create.Group",
         "Tab.ReadWrite.Group",
         "Member.Read.Group"
    ],
    "publishingState": "submitted",
    "lastModifiedDateTime": "2020-02-10 22:48:33.841",
}
```
