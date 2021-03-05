---
title: Список доменов
description: Извлечение списка объектов домена.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cb5d075b9802a44fb73f4c50bf61b90e8d7acb47
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441965"
---
# <a name="list-domains"></a><span data-ttu-id="e2cd6-103">Список доменов</span><span class="sxs-lookup"><span data-stu-id="e2cd6-103">List domains</span></span>

<span data-ttu-id="e2cd6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2cd6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e2cd6-105">Извлечение списка объектов домена.</span><span class="sxs-lookup"><span data-stu-id="e2cd6-105">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2cd6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2cd6-106">Permissions</span></span>
<span data-ttu-id="e2cd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2cd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2cd6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2cd6-109">Permission type</span></span>      | <span data-ttu-id="e2cd6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2cd6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2cd6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2cd6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e2cd6-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2cd6-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="e2cd6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2cd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2cd6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2cd6-114">Not supported.</span></span>    |
|<span data-ttu-id="e2cd6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2cd6-115">Application</span></span> | <span data-ttu-id="e2cd6-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2cd6-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2cd6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2cd6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2cd6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2cd6-118">Optional query parameters</span></span>
<span data-ttu-id="e2cd6-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2cd6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2cd6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2cd6-120">Request headers</span></span>
| <span data-ttu-id="e2cd6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e2cd6-121">Name</span></span>      |<span data-ttu-id="e2cd6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e2cd6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2cd6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2cd6-123">Authorization</span></span>  | <span data-ttu-id="e2cd6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2cd6-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e2cd6-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e2cd6-126">Accept</span></span>         | <span data-ttu-id="e2cd6-127">application/json;</span><span class="sxs-lookup"><span data-stu-id="e2cd6-127">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2cd6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2cd6-128">Request body</span></span>
<span data-ttu-id="e2cd6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2cd6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2cd6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2cd6-130">Response</span></span>

<span data-ttu-id="e2cd6-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [домена](../resources/domain.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e2cd6-131">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2cd6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e2cd6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2cd6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2cd6-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e2cd6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2cd6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains
```
# <a name="c"></a>[<span data-ttu-id="e2cd6-135">C#</span><span class="sxs-lookup"><span data-stu-id="e2cd6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domains-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2cd6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2cd6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domains-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2cd6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2cd6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domains-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2cd6-138">Java</span><span class="sxs-lookup"><span data-stu-id="e2cd6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domains-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e2cd6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2cd6-139">Response</span></span>
<span data-ttu-id="e2cd6-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2cd6-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "contoso.com",
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
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
