---
title: Публикация teamsapp
description: 'Публикация приложения в каталоге приложений Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1984ed7226da71ba1baf1bf15a7d83df4e6609a0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471651"
---
# <a name="publish-teamsapp"></a>Публикация teamsapp

Пространство имен: microsoft.graph

Публикация приложения [в](../resources/teamsapp.md) каталоге приложений Microsoft Teams.
В частности, этот API публикует приложение в каталог организации (каталог приложений клиента); созданный ресурс будет иметь **значение свойства distributionMethod** `organization` в .

Свойство **requiresReview** позволяет любому пользователю отправлять приложение для проверки администратором. Администраторы могут утверждать или отклонить эти приложения с помощью этого API или центра администрирования Microsoft Teams.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
|:----------------------------------     |:-------------|
| Делегированные (рабочая или учебная учетная запись) | AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается|
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

Публикация приложения, требуемая для проверки:

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
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

В теле запроса включите полезной нагрузкой манифест Teams zip. Дополнительные сведения см. [в материале Create an app package.](/microsoftteams/platform/concepts/apps/apps-package)

Каждое приложение в каталоге приложений должно иметь уникальный ID манифеста.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и [объект teamsApp.](../resources/teamsapp.md)

## <a name="examples"></a>Примеры

### <a name="example-1-publish-an-app-to-the-app-catalog"></a>Пример 1. Публикация приложения в каталоге приложений

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

---
Сведения о создании почтового файла приложения Microsoft Teams см. в статью [Создание пакета приложений.](/microsoftteams/platform/concepts/apps/apps-package)

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a>Пример 2. Отправка нового приложения для проверки в каталог приложений организации

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

---

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-3-approve-or-reject-an-app-pending-review"></a>Пример 3. Утверждение или отклонение приложения до рассмотрения

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
  "publishingState":"published"
}
```

---

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps('a761ad07-22ef-4a53-9feb-2837c8ad4a84')/appDefinitions/$entity",
    "id": "YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjUHVibGlzaGVk",
    "teamsAppId": "a761ad07-22ef-4a53-9feb-2837c8ad4a84",
    "azureADAppId": null,
    "displayName": "Ducks",
    "version": "1.1.8",
    "requiredResourceSpecificApplicationPermissions": [],
    "publishingState": "published",
    "shortDescription": "quaerat quasi magnam. slight change. 5",
    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
    "lastModifiedDateTime": null,
    "createdBy": null
}
```