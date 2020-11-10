---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0700729a30e6e58eaed8f3a90c87111bf3cfe971
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953642"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="3b999-103">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3b999-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="3b999-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b999-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b999-105">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3b999-105">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b999-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b999-106">Permissions</span></span>

<span data-ttu-id="3b999-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3b999-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b999-109">Permission type</span></span>      | <span data-ttu-id="3b999-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b999-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b999-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b999-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b999-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b999-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b999-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b999-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b999-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3b999-114">Not supported</span></span> |
|<span data-ttu-id="3b999-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b999-115">Application</span></span> |  <span data-ttu-id="3b999-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b999-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b999-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b999-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="3b999-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b999-118">Request headers</span></span>

| <span data-ttu-id="3b999-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3b999-119">Name</span></span> | <span data-ttu-id="3b999-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3b999-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3b999-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b999-121">Authorization</span></span> | <span data-ttu-id="3b999-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b999-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b999-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b999-124">Content-Type</span></span>  | <span data-ttu-id="3b999-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b999-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b999-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b999-126">Request body</span></span>
<span data-ttu-id="3b999-127">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b999-127">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3b999-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b999-128">Response</span></span>

<span data-ttu-id="3b999-129">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3b999-129">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b999-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3b999-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3b999-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b999-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3b999-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b999-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3b999-133">C#</span><span class="sxs-lookup"><span data-stu-id="3b999-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b999-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b999-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b999-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b999-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b999-136">Java</span><span class="sxs-lookup"><span data-stu-id="3b999-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3b999-137">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b999-137">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3b999-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b999-138">Response</span></span>

<span data-ttu-id="3b999-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b999-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


