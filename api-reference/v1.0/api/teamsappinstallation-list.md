---
title: Список приложений в группы
description: Получить список приложений, установленные в указанной группы.
ms.openlocfilehash: 6a9deb01e4874861b798ffcae32bebd77899fad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025031"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="37a81-103">Список приложений в группы</span><span class="sxs-lookup"><span data-stu-id="37a81-103">List apps in team</span></span>



<span data-ttu-id="37a81-104">Извлечь список [приложений установлен](../resources/teamsappinstallation.md) в указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="37a81-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37a81-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37a81-105">Permissions</span></span>

<span data-ttu-id="37a81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a81-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37a81-108">Permission type</span></span>      | <span data-ttu-id="37a81-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37a81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37a81-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37a81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37a81-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a81-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="37a81-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37a81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a81-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a81-113">Not supported.</span></span>    |
|<span data-ttu-id="37a81-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37a81-114">Application</span></span> | <span data-ttu-id="37a81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a81-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37a81-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37a81-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37a81-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37a81-117">Optional query parameters</span></span>

<span data-ttu-id="37a81-118">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="37a81-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37a81-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37a81-119">Request headers</span></span>

| <span data-ttu-id="37a81-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37a81-120">Header</span></span>       | <span data-ttu-id="37a81-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37a81-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37a81-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37a81-122">Authorization</span></span>  | <span data-ttu-id="37a81-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37a81-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37a81-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37a81-125">Request body</span></span>

<span data-ttu-id="37a81-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37a81-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37a81-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="37a81-127">Response</span></span>

<span data-ttu-id="37a81-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [teamsApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37a81-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37a81-129">Пример</span><span class="sxs-lookup"><span data-stu-id="37a81-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="37a81-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a81-130">Request</span></span>

<span data-ttu-id="37a81-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37a81-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="37a81-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="37a81-132">Response</span></span>

<span data-ttu-id="37a81-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37a81-133">The following is an example of the response.</span></span>
><span data-ttu-id="37a81-134">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="37a81-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="37a81-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37a81-135">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="37a81-136">Пример — начало имен установленные приложения</span><span class="sxs-lookup"><span data-stu-id="37a81-136">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="37a81-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a81-137">Request</span></span>

<span data-ttu-id="37a81-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37a81-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="37a81-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="37a81-139">Response</span></span>

<span data-ttu-id="37a81-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37a81-140">The following is an example of the response.</span></span>

><span data-ttu-id="37a81-141">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="37a81-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="37a81-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37a81-142">All the properties will be returned from an actual call.</span></span>
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