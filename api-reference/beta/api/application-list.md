---
title: Список приложений
description: Извлечь список приложений в данной организации.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 455a0ecd4d0a5f5c94c1edb083e0aa80c816b043
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971699"
---
# <a name="list-applications"></a><span data-ttu-id="0a5da-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="0a5da-103">List applications</span></span>

> <span data-ttu-id="0a5da-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a5da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a5da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a5da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a5da-106">Извлечь список приложений в данной организации.</span><span class="sxs-lookup"><span data-stu-id="0a5da-106">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a5da-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a5da-107">Permissions</span></span>
<span data-ttu-id="0a5da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a5da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0a5da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a5da-110">Permission type</span></span>      | <span data-ttu-id="0a5da-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a5da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a5da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a5da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0a5da-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0a5da-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0a5da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a5da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a5da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a5da-115">Not supported.</span></span>    |
|<span data-ttu-id="0a5da-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a5da-116">Application</span></span> | <span data-ttu-id="0a5da-117">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a5da-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a5da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a5da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a5da-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a5da-119">Optional query parameters</span></span>
<span data-ttu-id="0a5da-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0a5da-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a5da-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a5da-121">Request headers</span></span>
| <span data-ttu-id="0a5da-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0a5da-122">Name</span></span>       | <span data-ttu-id="0a5da-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0a5da-123">Type</span></span> | <span data-ttu-id="0a5da-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0a5da-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0a5da-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a5da-125">Authorization</span></span>  | <span data-ttu-id="0a5da-126">string</span><span class="sxs-lookup"><span data-stu-id="0a5da-126">string</span></span>  | <span data-ttu-id="0a5da-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a5da-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a5da-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a5da-129">Request body</span></span>
<span data-ttu-id="0a5da-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a5da-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a5da-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a5da-131">Response</span></span>

<span data-ttu-id="0a5da-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [приложения](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a5da-132">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a5da-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0a5da-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a5da-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a5da-134">Request</span></span>
<span data-ttu-id="0a5da-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a5da-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="0a5da-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a5da-136">Response</span></span>
<span data-ttu-id="0a5da-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0a5da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
