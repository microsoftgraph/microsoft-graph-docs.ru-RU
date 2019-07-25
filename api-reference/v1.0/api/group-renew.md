---
title: 'group: renew'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 264763a7f5997a989ad54056caa898a450f0da38
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885445"
---
# <a name="group-renew"></a><span data-ttu-id="8f465-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="8f465-104">group: renew</span></span>

<span data-ttu-id="8f465-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="8f465-105">Renews a group's expiration.</span></span> <span data-ttu-id="8f465-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="8f465-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f465-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f465-107">Permissions</span></span>

<span data-ttu-id="8f465-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f465-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="8f465-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f465-110">Permission type</span></span>      | <span data-ttu-id="8f465-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f465-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f465-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f465-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f465-113">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f465-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f465-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f465-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f465-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8f465-115">Not supported</span></span> |
|<span data-ttu-id="8f465-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f465-116">Application</span></span> | <span data-ttu-id="8f465-117">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f465-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f465-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f465-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="8f465-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f465-119">Request headers</span></span>
| <span data-ttu-id="8f465-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8f465-120">Name</span></span>       | <span data-ttu-id="8f465-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8f465-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8f465-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f465-122">Authorization</span></span>  | <span data-ttu-id="8f465-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8f465-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="8f465-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f465-124">Request body</span></span>

<span data-ttu-id="8f465-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f465-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f465-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f465-126">Response</span></span>

<span data-ttu-id="8f465-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8f465-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f465-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8f465-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8f465-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f465-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f465-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f465-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f465-132">C#</span><span class="sxs-lookup"><span data-stu-id="8f465-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f465-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f465-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f465-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f465-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f465-135">Java</span><span class="sxs-lookup"><span data-stu-id="8f465-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8f465-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f465-136">Response</span></span>
<span data-ttu-id="8f465-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f465-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
