---
title: Перечисление приложений, установленных для пользователя
description: Получение списка приложений, установленных в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7e8fb8a65ec71665477f734930ed0a40f6e74f3f
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606981"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="49d77-103">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="49d77-103">List apps installed for user</span></span>

<span data-ttu-id="49d77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49d77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49d77-105">Получение списка [приложений](../resources/teamsappinstallation.md) , установленных в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="49d77-105">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

> [!NOTE]
> <span data-ttu-id="49d77-106">`id`Ресурс **теамсаппинсталлатион** имеет не то же значение, что и `id` связанный ресурс **teamsApp** .</span><span class="sxs-lookup"><span data-stu-id="49d77-106">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="49d77-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49d77-107">Permissions</span></span>

<span data-ttu-id="49d77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49d77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49d77-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49d77-110">Permission type</span></span>      | <span data-ttu-id="49d77-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49d77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49d77-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49d77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49d77-113">Теамсаппинсталлатион. Реадфорусер, Теамсаппинсталлатион. Реадвритеселффорусер, Теамсаппинсталлатион. ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="49d77-113">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="49d77-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49d77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49d77-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49d77-115">Not supported.</span></span>    |
|<span data-ttu-id="49d77-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="49d77-116">Application</span></span> | <span data-ttu-id="49d77-117">Теамсаппинсталлатион. Реадфорусер. ALL, Теамсаппинсталлатион. Реадвритеселффорусер. ALL, Теамсаппинсталлатион. ReadWriteForUser. ALL</span><span class="sxs-lookup"><span data-stu-id="49d77-117">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49d77-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49d77-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49d77-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49d77-119">Optional query parameters</span></span>

<span data-ttu-id="49d77-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="49d77-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49d77-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49d77-121">Request headers</span></span>

| <span data-ttu-id="49d77-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49d77-122">Header</span></span>       | <span data-ttu-id="49d77-123">Значение</span><span class="sxs-lookup"><span data-stu-id="49d77-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="49d77-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49d77-124">Authorization</span></span>  | <span data-ttu-id="49d77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49d77-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49d77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49d77-127">Request body</span></span>

<span data-ttu-id="49d77-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49d77-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49d77-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="49d77-129">Response</span></span>

<span data-ttu-id="49d77-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49d77-130">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49d77-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="49d77-131">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="49d77-132">Пример 1: список приложений, установленных для указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="49d77-132">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="49d77-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="49d77-133">Request</span></span>

<span data-ttu-id="49d77-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49d77-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
```

#### <a name="response"></a><span data-ttu-id="49d77-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="49d77-135">Response</span></span>

<span data-ttu-id="49d77-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49d77-136">The following is an example of the response.</span></span>
><span data-ttu-id="49d77-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49d77-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk="
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="49d77-139">Пример 2: получение имен и других сведений о приложениях, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="49d77-139">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="49d77-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="49d77-140">Request</span></span>

<span data-ttu-id="49d77-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49d77-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_details"
} -->

```http
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="49d77-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="49d77-142">Response</span></span>

<span data-ttu-id="49d77-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49d77-143">The following is an example of the response.</span></span>

><span data-ttu-id="49d77-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49d77-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="49d77-146">Пример 3: получение ресурса установки приложения на основе идентификатора манифеста связанного приложения</span><span class="sxs-lookup"><span data-stu-id="49d77-146">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="49d77-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="49d77-147">Request</span></span>

<span data-ttu-id="49d77-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49d77-148">The following is an example of the request.</span></span> <span data-ttu-id="49d77-149">В этом примере идентификатор манифеста приложения Teams — "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee".</span><span class="sxs-lookup"><span data-stu-id="49d77-149">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_details_filter"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/97a5a533-833d-494b-b543-c0afe026cb96/teamwork/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```

#### <a name="response"></a><span data-ttu-id="49d77-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="49d77-150">Response</span></span>

<span data-ttu-id="49d77-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49d77-151">The following is an example of the response.</span></span>

><span data-ttu-id="49d77-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49d77-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details_filter",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=",
            "teamsApp": {
                "id": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
                "displayName": "YPA",
                "distributionMethod": "sideloaded"
            },
            "teamsAppDefinition": {
                "id": "MDI0MGEzNjgtMjVlMC00NTY5LThlYmUtMTM2MDFjYjU1YTE4IyM2LjAuMA==",
                "teamsAppId": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "azureADAppId": "9fc97ea2-c417-4c76-a2db-197612067b28",
                "displayName": "YPA",
                "version": "6.0.0",
                "requiredResourceSpecificApplicationPermissions": [
                ],
                "publishingState": "published",
                "shortdescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
                "description": "For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
    ]
}
```
## <a name="see-also"></a><span data-ttu-id="49d77-154">См. также</span><span class="sxs-lookup"><span data-stu-id="49d77-154">See also</span></span>
- [<span data-ttu-id="49d77-155">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="49d77-155">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User list teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
