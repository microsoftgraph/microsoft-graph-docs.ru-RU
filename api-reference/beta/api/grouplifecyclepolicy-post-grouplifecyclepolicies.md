---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d02a17677b5573431a1955b727a57877806d00ea
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419988"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="d9741-103">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d9741-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9741-104">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9741-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9741-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9741-105">Permissions</span></span>

<span data-ttu-id="d9741-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9741-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9741-108">Permission type</span></span>      | <span data-ttu-id="d9741-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9741-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9741-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9741-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9741-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9741-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9741-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9741-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9741-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d9741-113">Not supported</span></span> |
|<span data-ttu-id="d9741-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9741-114">Application</span></span> |  <span data-ttu-id="d9741-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9741-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9741-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9741-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="d9741-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9741-117">Request headers</span></span>

| <span data-ttu-id="d9741-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d9741-118">Name</span></span> | <span data-ttu-id="d9741-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d9741-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d9741-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9741-120">Authorization</span></span> | <span data-ttu-id="d9741-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9741-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9741-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9741-123">Content-Type</span></span>  | <span data-ttu-id="d9741-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9741-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9741-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9741-125">Request body</span></span>
<span data-ttu-id="d9741-126">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9741-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9741-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9741-127">Response</span></span>

<span data-ttu-id="d9741-128">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d9741-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9741-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d9741-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d9741-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9741-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d9741-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9741-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d9741-132">C#</span><span class="sxs-lookup"><span data-stu-id="d9741-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9741-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9741-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d9741-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d9741-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d9741-135">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9741-135">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d9741-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9741-136">Response</span></span>

<span data-ttu-id="d9741-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9741-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
