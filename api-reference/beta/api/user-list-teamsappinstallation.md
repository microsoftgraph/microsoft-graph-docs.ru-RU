---
title: Список приложений, установленных для пользователя
description: Получение списка приложений, установленных в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c31e731aba27fff245ecd92fc9d93d20d2c1fe27
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908553"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="4cabe-103">Список приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="4cabe-103">List apps installed for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cabe-104">Получение списка [приложений](../resources/teamsappinstallation.md) , установленных в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="4cabe-104">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4cabe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cabe-105">Permissions</span></span>

<span data-ttu-id="4cabe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cabe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cabe-108">Permission type</span></span>      | <span data-ttu-id="4cabe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cabe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cabe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cabe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4cabe-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cabe-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cabe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cabe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cabe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cabe-113">Not supported.</span></span>    |
|<span data-ttu-id="4cabe-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cabe-114">Application</span></span> | <span data-ttu-id="4cabe-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cabe-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4cabe-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cabe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cabe-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4cabe-117">Optional query parameters</span></span>

<span data-ttu-id="4cabe-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4cabe-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cabe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cabe-119">Request headers</span></span>

| <span data-ttu-id="4cabe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cabe-120">Header</span></span>       | <span data-ttu-id="4cabe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4cabe-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4cabe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cabe-122">Authorization</span></span>  | <span data-ttu-id="4cabe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cabe-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4cabe-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cabe-125">Request body</span></span>

<span data-ttu-id="4cabe-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cabe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cabe-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cabe-127">Response</span></span>

<span data-ttu-id="4cabe-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cabe-128">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cabe-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="4cabe-129">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="4cabe-130">Пример 1: список приложений, установленных для указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="4cabe-130">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="4cabe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cabe-131">Request</span></span>

<span data-ttu-id="4cabe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cabe-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
```

#### <a name="response"></a><span data-ttu-id="4cabe-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cabe-133">Response</span></span>

<span data-ttu-id="4cabe-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4cabe-134">The following is an example of the response.</span></span>
><span data-ttu-id="4cabe-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cabe-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "id-value"
    }
  ]
}
```
### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="4cabe-137">Пример 2: получение имен и других сведений о приложениях, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="4cabe-137">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="4cabe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cabe-138">Request</span></span>

<span data-ttu-id="4cabe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cabe-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="4cabe-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cabe-140">Response</span></span>

<span data-ttu-id="4cabe-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4cabe-141">The following is an example of the response.</span></span>

><span data-ttu-id="4cabe-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cabe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User list teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
