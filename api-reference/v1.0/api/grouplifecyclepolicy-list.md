---
title: Перечисление groupLifecyclePolicies
description: Перечисление всех объектов groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a6a7a04d112dc74bed9f4d33c016ad0c1731bd66
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263569"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="75a88-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="75a88-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="75a88-104">Список всех объектов [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="75a88-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="75a88-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75a88-105">Permissions</span></span>

<span data-ttu-id="75a88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="75a88-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75a88-108">Permission type</span></span>      | <span data-ttu-id="75a88-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75a88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75a88-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75a88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="75a88-111">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a88-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="75a88-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75a88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75a88-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a88-113">Not supported.</span></span>    |
|<span data-ttu-id="75a88-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75a88-114">Application</span></span> | <span data-ttu-id="75a88-115">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a88-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75a88-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75a88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="75a88-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75a88-117">Optional query parameters</span></span>
<span data-ttu-id="75a88-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75a88-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75a88-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75a88-119">Request headers</span></span>
| <span data-ttu-id="75a88-120">Имя</span><span class="sxs-lookup"><span data-stu-id="75a88-120">Name</span></span> | <span data-ttu-id="75a88-121">Описание</span><span class="sxs-lookup"><span data-stu-id="75a88-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="75a88-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75a88-122">Authorization</span></span> | <span data-ttu-id="75a88-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a88-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75a88-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75a88-125">Request body</span></span>
<span data-ttu-id="75a88-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75a88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75a88-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="75a88-127">Response</span></span>

<span data-ttu-id="75a88-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75a88-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a88-129">Пример</span><span class="sxs-lookup"><span data-stu-id="75a88-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="75a88-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="75a88-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="75a88-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a88-131">Response</span></span>

<span data-ttu-id="75a88-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75a88-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="75a88-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="75a88-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="75a88-135">C#</span><span class="sxs-lookup"><span data-stu-id="75a88-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="75a88-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="75a88-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="75a88-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="75a88-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
