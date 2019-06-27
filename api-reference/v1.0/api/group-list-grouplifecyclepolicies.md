---
title: Перечисление groupLifecyclePolicies
description: Получает список объектов groupLifecyclePolicy, к которым принадлежит группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5ace0257e6bf8389fc3149947903bfd7d64f4e82
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273523"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="e1499-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="e1499-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="e1499-104">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="e1499-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1499-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1499-105">Permissions</span></span>

<span data-ttu-id="e1499-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1499-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1499-108">Permission type</span></span>      | <span data-ttu-id="e1499-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1499-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1499-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1499-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1499-111">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1499-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e1499-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1499-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1499-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1499-113">Not supported.</span></span>    |
|<span data-ttu-id="e1499-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1499-114">Application</span></span> | <span data-ttu-id="e1499-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1499-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1499-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1499-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e1499-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1499-117">Optional query parameters</span></span>
<span data-ttu-id="e1499-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1499-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1499-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1499-119">Request headers</span></span>
| <span data-ttu-id="e1499-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e1499-120">Name</span></span> | <span data-ttu-id="e1499-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e1499-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="e1499-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1499-122">Authorization</span></span> | <span data-ttu-id="e1499-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1499-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1499-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1499-125">Request body</span></span>
<span data-ttu-id="e1499-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1499-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e1499-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1499-127">Response</span></span>
<span data-ttu-id="e1499-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1499-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1499-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e1499-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e1499-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1499-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="e1499-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1499-131">Response</span></span>

<span data-ttu-id="e1499-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1499-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1499-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e1499-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1499-135">C#</span><span class="sxs-lookup"><span data-stu-id="e1499-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1499-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1499-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e1499-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e1499-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
