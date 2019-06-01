---
title: Список доменов
description: Получение списка объектов Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 714eb13377ee613b19812c42a2edc19726c941c9
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655623"
---
# <a name="list-domains"></a><span data-ttu-id="e9787-103">Список доменов</span><span class="sxs-lookup"><span data-stu-id="e9787-103">List domains</span></span>

<span data-ttu-id="e9787-104">Получение списка объектов Domain.</span><span class="sxs-lookup"><span data-stu-id="e9787-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9787-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9787-105">Permissions</span></span>
<span data-ttu-id="e9787-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9787-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9787-108">Permission type</span></span>      | <span data-ttu-id="e9787-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9787-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9787-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9787-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9787-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9787-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="e9787-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9787-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9787-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9787-113">Not supported.</span></span>    |
|<span data-ttu-id="e9787-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9787-114">Application</span></span> | <span data-ttu-id="e9787-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9787-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9787-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9787-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9787-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9787-117">Optional query parameters</span></span>
<span data-ttu-id="e9787-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e9787-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9787-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9787-119">Request headers</span></span>
| <span data-ttu-id="e9787-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e9787-120">Name</span></span>      |<span data-ttu-id="e9787-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e9787-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9787-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9787-122">Authorization</span></span>  | <span data-ttu-id="e9787-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9787-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e9787-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9787-125">Accept</span></span>         | <span data-ttu-id="e9787-126">приложение/JSON;</span><span class="sxs-lookup"><span data-stu-id="e9787-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9787-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9787-127">Request body</span></span>
<span data-ttu-id="e9787-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9787-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9787-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9787-129">Response</span></span>

<span data-ttu-id="e9787-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domain](../resources/domain.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9787-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9787-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e9787-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9787-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9787-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="e9787-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9787-133">Response</span></span>
<span data-ttu-id="e9787-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9787-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9787-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e9787-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e9787-137">C#</span><span class="sxs-lookup"><span data-stu-id="e9787-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domains-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9787-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9787-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domains-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
