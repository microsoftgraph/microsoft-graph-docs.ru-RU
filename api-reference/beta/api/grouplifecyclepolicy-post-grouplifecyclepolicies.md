---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f022be2e393f10805e9d62c49a6dbfd8333d93e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442610"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="36771-103">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="36771-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36771-104">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="36771-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="36771-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36771-105">Permissions</span></span>

<span data-ttu-id="36771-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="36771-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36771-108">Permission type</span></span>      | <span data-ttu-id="36771-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36771-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36771-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36771-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36771-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36771-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="36771-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36771-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36771-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="36771-113">Not supported</span></span> |
|<span data-ttu-id="36771-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36771-114">Application</span></span> |  <span data-ttu-id="36771-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36771-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36771-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36771-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="36771-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36771-117">Request headers</span></span>

| <span data-ttu-id="36771-118">Имя</span><span class="sxs-lookup"><span data-stu-id="36771-118">Name</span></span> | <span data-ttu-id="36771-119">Описание</span><span class="sxs-lookup"><span data-stu-id="36771-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="36771-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36771-120">Authorization</span></span> | <span data-ttu-id="36771-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36771-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36771-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36771-123">Content-Type</span></span>  | <span data-ttu-id="36771-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36771-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="36771-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36771-125">Request body</span></span>
<span data-ttu-id="36771-126">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36771-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="36771-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="36771-127">Response</span></span>

<span data-ttu-id="36771-128">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36771-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36771-129">Пример</span><span class="sxs-lookup"><span data-stu-id="36771-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="36771-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="36771-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="36771-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="36771-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="36771-132">C#</span><span class="sxs-lookup"><span data-stu-id="36771-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36771-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="36771-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36771-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="36771-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="36771-135">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36771-135">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="36771-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="36771-136">Response</span></span>

<span data-ttu-id="36771-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36771-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
