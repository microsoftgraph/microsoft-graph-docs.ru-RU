---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9dd1489714c4de87f0072ef0498c5acdf008d5ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938827"
---
# <a name="list-organization"></a><span data-ttu-id="23aab-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="23aab-103">List organization</span></span>

> <span data-ttu-id="23aab-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23aab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23aab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23aab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23aab-106">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="23aab-106">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="23aab-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23aab-107">Permissions</span></span>
<span data-ttu-id="23aab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23aab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23aab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23aab-110">Permission type</span></span>      | <span data-ttu-id="23aab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23aab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23aab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23aab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23aab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23aab-113">Not supported.</span></span>    |
|<span data-ttu-id="23aab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23aab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23aab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23aab-115">Not supported.</span></span>    |
|<span data-ttu-id="23aab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23aab-116">Application</span></span> | <span data-ttu-id="23aab-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23aab-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23aab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23aab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23aab-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23aab-119">Optional query parameters</span></span>
<span data-ttu-id="23aab-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23aab-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23aab-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23aab-121">Request headers</span></span>
| <span data-ttu-id="23aab-122">Имя</span><span class="sxs-lookup"><span data-stu-id="23aab-122">Name</span></span>       | <span data-ttu-id="23aab-123">Тип</span><span class="sxs-lookup"><span data-stu-id="23aab-123">Type</span></span> | <span data-ttu-id="23aab-124">Описание</span><span class="sxs-lookup"><span data-stu-id="23aab-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23aab-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="23aab-125">Authorization</span></span>  | <span data-ttu-id="23aab-126">string</span><span class="sxs-lookup"><span data-stu-id="23aab-126">string</span></span>  | <span data-ttu-id="23aab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23aab-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23aab-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23aab-129">Request body</span></span>
<span data-ttu-id="23aab-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23aab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23aab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="23aab-131">Response</span></span>

<span data-ttu-id="23aab-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23aab-132">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23aab-133">Пример</span><span class="sxs-lookup"><span data-stu-id="23aab-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23aab-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="23aab-134">Request</span></span>
<span data-ttu-id="23aab-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23aab-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="23aab-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="23aab-136">Response</span></span>
<span data-ttu-id="23aab-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="23aab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
