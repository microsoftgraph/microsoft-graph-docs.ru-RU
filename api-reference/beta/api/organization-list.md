---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c119d755ca4fd9a795fd8eff70b9bb015dbc7829
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511886"
---
# <a name="list-organization"></a><span data-ttu-id="f1ed6-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="f1ed6-103">List organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1ed6-104">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1ed6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1ed6-105">Permissions</span></span>
<span data-ttu-id="f1ed6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ed6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1ed6-108">Permission type</span></span>      | <span data-ttu-id="f1ed6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1ed6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1ed6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1ed6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1ed6-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-111">Not supported.</span></span>    |
|<span data-ttu-id="f1ed6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1ed6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1ed6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-113">Not supported.</span></span>    |
|<span data-ttu-id="f1ed6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1ed6-114">Application</span></span> | <span data-ttu-id="f1ed6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1ed6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1ed6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1ed6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f1ed6-117">Optional query parameters</span></span>
<span data-ttu-id="f1ed6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f1ed6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1ed6-119">Request headers</span></span>
| <span data-ttu-id="f1ed6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f1ed6-120">Name</span></span>       | <span data-ttu-id="f1ed6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f1ed6-121">Type</span></span> | <span data-ttu-id="f1ed6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f1ed6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f1ed6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1ed6-123">Authorization</span></span>  | <span data-ttu-id="f1ed6-124">string</span><span class="sxs-lookup"><span data-stu-id="f1ed6-124">string</span></span>  | <span data-ttu-id="f1ed6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1ed6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1ed6-127">Request body</span></span>
<span data-ttu-id="f1ed6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1ed6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1ed6-129">Response</span></span>

<span data-ttu-id="f1ed6-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-130">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1ed6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f1ed6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1ed6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1ed6-132">Request</span></span>
<span data-ttu-id="f1ed6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1ed6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="f1ed6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1ed6-134">Response</span></span>
<span data-ttu-id="f1ed6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f1ed6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
