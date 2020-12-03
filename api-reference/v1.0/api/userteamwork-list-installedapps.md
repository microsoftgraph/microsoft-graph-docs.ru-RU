---
title: Перечисление приложений, установленных для пользователя
description: Получение списка приложений, установленных в личной области указанного пользователя.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0f44fdc43328507a4cf156ce25d528b1c2bb8d6d
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564087"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="68c0b-103">Перечисление приложений, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="68c0b-103">List apps installed for user</span></span>

<span data-ttu-id="68c0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68c0b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68c0b-105">Получение списка [приложений](../resources/teamsappinstallation.md) , установленных в личной области указанного [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="68c0b-105">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68c0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68c0b-106">Permissions</span></span>

<span data-ttu-id="68c0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68c0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68c0b-109">Permission type</span></span>      | <span data-ttu-id="68c0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68c0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68c0b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68c0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="68c0b-112">Теамсаппинсталлатион. Реадфорусер, Теамсаппинсталлатион. Read, Теамсаппинсталлатион. Реадвритеселффорусер, TeamsAppInstallation. ReadWriteForUser, TeamsAppInstallation. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68c0b-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.Read, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="68c0b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68c0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68c0b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c0b-114">Not supported.</span></span>    |
|<span data-ttu-id="68c0b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="68c0b-115">Application</span></span> | <span data-ttu-id="68c0b-116">Теамсаппинсталлатион. Реадфорусер. ALL, Теамсаппинсталлатион. Read. ALL, Теамсаппинсталлатион. Реадвритеселффорусер. ALL, TeamsAppInstallation. ReadWriteForUser. ALL, TeamsAppInstallation. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="68c0b-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.Read.All,TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68c0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68c0b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68c0b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68c0b-118">Optional query parameters</span></span>

<span data-ttu-id="68c0b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="68c0b-119">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68c0b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68c0b-120">Request headers</span></span>

| <span data-ttu-id="68c0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68c0b-121">Header</span></span>       | <span data-ttu-id="68c0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68c0b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68c0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68c0b-123">Authorization</span></span>  | <span data-ttu-id="68c0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68c0b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68c0b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68c0b-126">Request body</span></span>

<span data-ttu-id="68c0b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68c0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68c0b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c0b-128">Response</span></span>

<span data-ttu-id="68c0b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68c0b-129">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68c0b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="68c0b-130">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="68c0b-131">Пример 1: список приложений, установленных для указанного пользователя</span><span class="sxs-lookup"><span data-stu-id="68c0b-131">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="68c0b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="68c0b-132">Request</span></span>

<span data-ttu-id="68c0b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68c0b-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
```

#### <a name="response"></a><span data-ttu-id="68c0b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c0b-134">Response</span></span>

<span data-ttu-id="68c0b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68c0b-135">The following is an example of the response.</span></span>
><span data-ttu-id="68c0b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68c0b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="68c0b-138">Пример 2: получение имен и других сведений о приложениях, установленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="68c0b-138">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="68c0b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="68c0b-139">Request</span></span>

<span data-ttu-id="68c0b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68c0b-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
} -->

```http
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="68c0b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c0b-141">Response</span></span>

<span data-ttu-id="68c0b-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68c0b-142">The following is an example of the response.</span></span>

><span data-ttu-id="68c0b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68c0b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
