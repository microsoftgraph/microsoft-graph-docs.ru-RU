---
title: Список доменов
description: Получение списка объектов Domain.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 503655b7a12c33584db8a4473187f88d7185c36b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180027"
---
# <a name="list-domains"></a><span data-ttu-id="ed78c-103">Список доменов</span><span class="sxs-lookup"><span data-stu-id="ed78c-103">List domains</span></span>

<span data-ttu-id="ed78c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed78c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed78c-105">Получение списка объектов Domain.</span><span class="sxs-lookup"><span data-stu-id="ed78c-105">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed78c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed78c-106">Permissions</span></span>
<span data-ttu-id="ed78c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed78c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed78c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed78c-109">Permission type</span></span>      | <span data-ttu-id="ed78c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed78c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed78c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed78c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed78c-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed78c-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="ed78c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed78c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed78c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed78c-114">Not supported.</span></span>    |
|<span data-ttu-id="ed78c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed78c-115">Application</span></span> | <span data-ttu-id="ed78c-116">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed78c-116">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed78c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed78c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed78c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ed78c-118">Optional query parameters</span></span>
<span data-ttu-id="ed78c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ed78c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed78c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed78c-120">Request headers</span></span>
| <span data-ttu-id="ed78c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ed78c-121">Name</span></span>      |<span data-ttu-id="ed78c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ed78c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed78c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed78c-123">Authorization</span></span>  | <span data-ttu-id="ed78c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed78c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ed78c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ed78c-126">Accept</span></span>         | <span data-ttu-id="ed78c-127">приложение/JSON;</span><span class="sxs-lookup"><span data-stu-id="ed78c-127">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed78c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed78c-128">Request body</span></span>
<span data-ttu-id="ed78c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed78c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed78c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed78c-130">Response</span></span>

<span data-ttu-id="ed78c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domain](../resources/domain.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed78c-131">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed78c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ed78c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed78c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed78c-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed78c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed78c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains
```
# <a name="c"></a>[<span data-ttu-id="ed78c-135">C#</span><span class="sxs-lookup"><span data-stu-id="ed78c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed78c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed78c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed78c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed78c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ed78c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed78c-138">Response</span></span>
<span data-ttu-id="ed78c-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed78c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
