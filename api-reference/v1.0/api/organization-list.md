---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0fbd38f4d3c0e4ceec9f025e9822b635ce6a0d54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939163"
---
# <a name="list-organization"></a><span data-ttu-id="57ca3-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="57ca3-103">List organization</span></span>



<span data-ttu-id="57ca3-104">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="57ca3-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="57ca3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57ca3-105">Permissions</span></span>
<span data-ttu-id="57ca3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ca3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57ca3-108">Permission type</span></span>      | <span data-ttu-id="57ca3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57ca3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57ca3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57ca3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57ca3-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ca3-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="57ca3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57ca3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57ca3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ca3-113">Not supported.</span></span>    |
|<span data-ttu-id="57ca3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57ca3-114">Application</span></span> | <span data-ttu-id="57ca3-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ca3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="57ca3-116">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="57ca3-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="57ca3-117">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="57ca3-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="57ca3-118">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="57ca3-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="57ca3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57ca3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57ca3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57ca3-120">Optional query parameters</span></span>
<span data-ttu-id="57ca3-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57ca3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="57ca3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57ca3-122">Request headers</span></span>
| <span data-ttu-id="57ca3-123">Имя</span><span class="sxs-lookup"><span data-stu-id="57ca3-123">Name</span></span>       | <span data-ttu-id="57ca3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="57ca3-124">Type</span></span> | <span data-ttu-id="57ca3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="57ca3-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="57ca3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="57ca3-126">Authorization</span></span>  | <span data-ttu-id="57ca3-127">строка</span><span class="sxs-lookup"><span data-stu-id="57ca3-127">string</span></span>  | <span data-ttu-id="57ca3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57ca3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57ca3-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57ca3-130">Request body</span></span>
<span data-ttu-id="57ca3-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57ca3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57ca3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ca3-132">Response</span></span>

<span data-ttu-id="57ca3-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57ca3-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57ca3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="57ca3-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57ca3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="57ca3-135">Request</span></span>
<span data-ttu-id="57ca3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57ca3-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="57ca3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ca3-137">Response</span></span>
<span data-ttu-id="57ca3-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="57ca3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
