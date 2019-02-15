---
title: Список приложений в команде
description: Получение списка приложений, установленных в указанной команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 749a0c0e0c3a93b54487d9dea8823ad59a2658fd
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057010"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="dfa0a-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="dfa0a-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa0a-104">Получение списка приложений, [установленных](../resources/teamsappinstallation.md) в указанной [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="dfa0a-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfa0a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa0a-105">Permissions</span></span>

<span data-ttu-id="dfa0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa0a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa0a-108">Permission type</span></span>      | <span data-ttu-id="dfa0a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfa0a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfa0a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfa0a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dfa0a-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa0a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfa0a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfa0a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa0a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-113">Not supported.</span></span>    |
|<span data-ttu-id="dfa0a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfa0a-114">Application</span></span> | <span data-ttu-id="dfa0a-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa0a-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="dfa0a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfa0a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfa0a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfa0a-117">Optional query parameters</span></span>

<span data-ttu-id="dfa0a-118">Этот метод поддерживает [параметры запросов](/graph/query-parameters) $filter, $select и $Expand OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfa0a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfa0a-119">Request headers</span></span>

| <span data-ttu-id="dfa0a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfa0a-120">Header</span></span>       | <span data-ttu-id="dfa0a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dfa0a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dfa0a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfa0a-122">Authorization</span></span>  | <span data-ttu-id="dfa0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfa0a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfa0a-125">Request body</span></span>

<span data-ttu-id="dfa0a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfa0a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfa0a-127">Response</span></span>

<span data-ttu-id="dfa0a-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfa0a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dfa0a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfa0a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa0a-130">Request</span></span>

<span data-ttu-id="dfa0a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="dfa0a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa0a-132">Response</span></span>

<span data-ttu-id="dfa0a-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-133">The following is an example of the response.</span></span>
><span data-ttu-id="dfa0a-134">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dfa0a-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-135">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="dfa0a-136">Пример: извлечение имен установленных приложений</span><span class="sxs-lookup"><span data-stu-id="dfa0a-136">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="dfa0a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa0a-137">Request</span></span>

<span data-ttu-id="dfa0a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="dfa0a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa0a-139">Response</span></span>

<span data-ttu-id="dfa0a-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-140">The following is an example of the response.</span></span>

><span data-ttu-id="dfa0a-141">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dfa0a-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfa0a-142">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
