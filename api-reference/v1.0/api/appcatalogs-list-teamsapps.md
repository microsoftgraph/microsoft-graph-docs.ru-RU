---
title: Перечисление teamsApp
description: Список Teams приложений, опубликованных в каталоге приложений клиента.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7b2106e86cc2a3a719b88311b23b3a632a24c4c7
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366116"
---
# <a name="list-teamsapp"></a>Перечисление teamsApp

Пространство имен: microsoft.graph

Вывод [списка приложений](../resources/teamsapp.md) из Microsoft Teams приложения.
К ним относятся приложения из Microsoft Teams, а также приложения из каталога приложений организации (каталог приложений клиента). Чтобы получить приложения только из каталога приложений организации, `organization` укажите в запросе **значение distributionMethod** .

> [!NOTE]
> Ресурс `id` **teamsApp** `id` создается сервером и не совпадает с указанным в манифесте Teams приложения. Предоставляемый `id` разработчиком как часть манифеста Teams приложения `externalId` помечается как ресурс **teamsApp**.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All **, Directory.ReadWrite.All** |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | AppCatalog.Read.All, AppCatalog.ReadWrite.All |

> **Примечание**. Разрешения, отмеченные **, поддерживаются только для обратной совместимости. Рекомендуется обновить решения, чтобы использовать другое разрешение, указанное в предыдущей таблице, и избегать использования этих разрешений в будущем.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.

При `$expand=AppDefinitions` использовании будут возвращены дополнительные сведения о состоянии приложения, такие как **publishingState**, которое отражает состояние проверки отправки приложения и возвращает, было ли приложение утверждено, отклонено или остается на проверке. 

> **Примечание:** Чтобы сократить список результатов, можно выполнить фильтрацию по любому из полей объекта [teamsApp](../resources/teamsapp.md) . Можно использовать любую из следующих операций фильтра: "Равно", "Не равно" или "нет".

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и список объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a>Пример 1. Вывод списка всех приложений, которые относятся к клиенту

В следующем примере перечислены все приложения, относящиеся к вашему клиенту.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapps-filter-distributionmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapps-filter-distributionmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapps-filter-distributionmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapps-filter-distributionmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapps-filter-distributionmethod-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-teamsapps-filter-distributionmethod-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a>Пример 2. Перечисление приложений с заданным идентификатором

В следующем примере перечислены приложения с заданным идентификатором.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-filter-id-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-teamsapp-filter-id-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a>Пример 3. Поиск приложения на основе Teams манифеста приложения.

В следующем примере перечислены приложения, соответствующие идентификатору, указанному в Teams приложения. В этом примере идентификатор манифеста приложения Teams — 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-filter-externalid-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-teamsapp-filter-externalid-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps",
    "value": [
        {
            "id": "22f73bbe-f67a-4dea-bd54-54cac718cb2b",
            "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName": "YPA",
            "distributionMethod": "organization"
        }
    ]
}
```

### <a name="example-4-list-applications-with-a-given-id-and-return-the-submission-review-state"></a>Пример 4. Перечисление приложений с заданным идентификатором и возврат состояния проверки отправки

В следующем примере перечислены приложения с заданным идентификатором и **развернутые объекты appDefinitions** , чтобы получить **значение publishingState**, которое отражает состояние проверки отправки приложения. `Submitted` означает, что проверка находится в состоянии ожидания, означает, `published` что приложение было утверждено администратором, и означает, `rejected` что приложение было отклонено администратором.

#### <a name="request"></a>Запрос



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_with_filter_expand_appdefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-with-filter-expand-appdefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-with-filter-expand-appdefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-with-filter-expand-appdefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-with-filter-expand-appdefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-with-filter-expand-appdefinitions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-teamsapp-with-filter-expand-appdefinitions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_with_filter_expand_appdefinitions",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "876df28f-2e78-423b-94a5-44181bd0e225",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization",
      "appDefinitions": [
        {
          "id": "NGQyMGNiNDUtZWViYS00ZTEyLWE3YzktMGQ0NDgzYjYxNzU2IyMxLjAuMA==",
          "teamsAppId": "876df28f-2e78-423b-94a5-44181bd0e225",
          "azureADAppId": null,
          "displayName": "Test App",
          "version": "1.0.1",
          "requiredResourceSpecificApplicationPermissions": [],
          "publishingState": "published"
        }
      ]
    }
  ]
}
```

### <a name="example-5-list-the-details-of-only-those-apps-in-the-catalog-that-contain-a-bot"></a>Пример 5. Вывод списка сведений только о приложениях в каталоге, содержащих бота

В следующем примере перечислены только те приложения в каталоге, которые содержат бота.

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_with_bots"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$expand=appDefinitions($expand=bot)&$filter=appDefinitions/any(a:a/bot ne null)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-with-bots-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-with-bots-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-with-bots-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-with-bots-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-teamsapp-with-bots-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-teamsapp-with-bots-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "name": "list_teamsapp_with_bots",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps(appDefinitions(bot()))",
    "value": [
        {
            "id": "8a1ed7a3-5c78-46b2-8504-f9da00a1d1a6",
            "externalId": "3CAB7543-216D-47C6-986C-6247670F4663",
            "displayName": "Ducks-3",
            "distributionMethod": "organization",
            "appDefinitions": [
                {
                    "@odata.etag": "ImNOTW1CR2V1VzgwczlEblVidU00UHc9PSI=",
                    "id": "OGExZWQ3YTMtNWM3OC00NmIyLTg1MDQtZjlkYTAwYTFkMWE2IyMxLjAuOSMjUmVqZWN0ZWQ=",
                    "teamsAppId": "8a1ed7a3-5c78-46b2-8504-f9da00a1d1a6",
                    "azureADAppId": null,
                    "displayName": "Ducks-3",
                    "version": "1.0.9",
                    "requiredResourceSpecificApplicationPermissions": [],
                    "publishingState": "rejected",
                    "shortDescription": "quaerat quasi magnam. slight change. 5",
                    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
                    "lastModifiedDateTime": "2020-11-23T21:36:00.9437445Z",
                    "createdBy": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "70292a90-d2a7-432c-857e-55db6d8f5cd0",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    },
                    "bot": {
                        "id": "bb9f67a4-893b-48d7-ab17-40ed466c0f16"
                    }
                }
            ]
        },
        {
            "id": "30909dee-f7dd-4f89-8b3b-55de2e32489c",
            "externalId": "0ebd3f4d-ca91-495b-a227-a17d298e22cc",
            "displayName": "Self-Install-App-E2E-Tests",
            "distributionMethod": "organization",
            "appDefinitions": [
                {
                    "@odata.etag": "IkwzVDlMOTBSSEdTMFducHUyYkpjVmc9PSI=",
                    "id": "MzA5MDlkZWUtZjdkZC00Zjg5LThiM2ItNTVkZTJlMzI0ODljIyM2LjAuMCMjU3VibWl0dGVk",
                    "teamsAppId": "30909dee-f7dd-4f89-8b3b-55de2e32489c",
                    "azureADAppId": "d75abc57-8255-4309-9c29-a3c689e20341",
                    "displayName": "Self-Install-App-E2E-Tests",
                    "version": "6.0.0",
                    "requiredResourceSpecificApplicationPermissions": [],
                    "publishingState": "submitted",
                    "shortDescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
                    "description": "For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
                    "lastModifiedDateTime": "2020-08-25T18:40:13.035341Z",
                    "createdBy": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "c071a180-a220-43a1-adaf-e8db95c4a7d6",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    },
                    "bot": {
                        "id": "da7d471b-de7d-4152-8556-1cdf7a564f6c"
                    }
                }
            ]
        }
    ]
}
```
## <a name="see-also"></a>См. также

- [Перечисление приложений, установленных в команде](team-list-installedapps.md) <!-- - [List apps installed in a chat](chat-list-installedapps.md) -->
- [Перечисление приложений, установленных в личной области пользователя](userteamwork-list-installedapps.md)

