---
title: Список приложений в группы
description: Получить список приложений, установленные в указанной группы.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02f324c17bde34973c6f3fe612c327a0f7488eb4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957643"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="51d4e-103">Список приложений в группы</span><span class="sxs-lookup"><span data-stu-id="51d4e-103">List apps in team</span></span>

> <span data-ttu-id="51d4e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51d4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51d4e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51d4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51d4e-106">Извлечь список [приложений установлен](../resources/teamsappinstallation.md) в указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="51d4e-106">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="51d4e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51d4e-107">Permissions</span></span>

<span data-ttu-id="51d4e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51d4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51d4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51d4e-110">Permission type</span></span>      | <span data-ttu-id="51d4e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51d4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51d4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51d4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51d4e-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51d4e-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="51d4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51d4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51d4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51d4e-115">Not supported.</span></span>    |
|<span data-ttu-id="51d4e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51d4e-116">Application</span></span> | <span data-ttu-id="51d4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51d4e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51d4e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51d4e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51d4e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51d4e-119">Optional query parameters</span></span>

<span data-ttu-id="51d4e-120">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51d4e-120">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51d4e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51d4e-121">Request headers</span></span>

| <span data-ttu-id="51d4e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51d4e-122">Header</span></span>       | <span data-ttu-id="51d4e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="51d4e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51d4e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51d4e-124">Authorization</span></span>  | <span data-ttu-id="51d4e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51d4e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51d4e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51d4e-127">Request body</span></span>

<span data-ttu-id="51d4e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51d4e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51d4e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51d4e-129">Response</span></span>

<span data-ttu-id="51d4e-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [teamsApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="51d4e-130">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51d4e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51d4e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="51d4e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51d4e-132">Request</span></span>

<span data-ttu-id="51d4e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51d4e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="51d4e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="51d4e-134">Response</span></span>

<span data-ttu-id="51d4e-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="51d4e-135">The following is an example of the response.</span></span>
><span data-ttu-id="51d4e-136">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="51d4e-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51d4e-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51d4e-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="51d4e-138">Пример — начало имен установленные приложения</span><span class="sxs-lookup"><span data-stu-id="51d4e-138">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="51d4e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="51d4e-139">Request</span></span>

<span data-ttu-id="51d4e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51d4e-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="51d4e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="51d4e-141">Response</span></span>

<span data-ttu-id="51d4e-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="51d4e-142">The following is an example of the response.</span></span>

><span data-ttu-id="51d4e-143">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="51d4e-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51d4e-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51d4e-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
