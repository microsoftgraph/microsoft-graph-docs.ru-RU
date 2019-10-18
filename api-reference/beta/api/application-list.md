---
title: Список приложений
description: Получение списка приложений в этой организации.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1642eac11159ac016669ecb9b9c058c7eb4ca1de
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719033"
---
# <a name="list-applications"></a><span data-ttu-id="2d161-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="2d161-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d161-104">Получение списка приложений в этой организации.</span><span class="sxs-lookup"><span data-stu-id="2d161-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d161-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d161-105">Permissions</span></span>
<span data-ttu-id="2d161-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2d161-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d161-108">Permission type</span></span>      | <span data-ttu-id="2d161-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d161-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d161-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d161-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d161-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d161-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d161-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d161-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d161-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d161-113">Not supported.</span></span>    |
|<span data-ttu-id="2d161-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d161-114">Application</span></span> | <span data-ttu-id="2d161-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d161-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d161-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d161-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2d161-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d161-117">Optional query parameters</span></span>
<span data-ttu-id="2d161-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2d161-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d161-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d161-119">Request headers</span></span>
| <span data-ttu-id="2d161-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2d161-120">Name</span></span>       | <span data-ttu-id="2d161-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2d161-121">Type</span></span> | <span data-ttu-id="2d161-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d161-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2d161-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d161-123">Authorization</span></span>  | <span data-ttu-id="2d161-124">string</span><span class="sxs-lookup"><span data-stu-id="2d161-124">string</span></span>  | <span data-ttu-id="2d161-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d161-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d161-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d161-127">Request body</span></span>
<span data-ttu-id="2d161-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d161-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d161-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d161-129">Response</span></span>

<span data-ttu-id="2d161-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d161-130">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d161-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2d161-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d161-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d161-132">Request</span></span>
<span data-ttu-id="2d161-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d161-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2d161-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d161-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d161-135">C#</span><span class="sxs-lookup"><span data-stu-id="2d161-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d161-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d161-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d161-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d161-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d161-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d161-138">Response</span></span>
<span data-ttu-id="2d161-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d161-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
