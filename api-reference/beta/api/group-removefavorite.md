---
title: 'group: removeFavorite'
description: Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для групп Microsoft 365.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4409fe7b777e470f6e25fa5c675335512bf58433
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786951"
---
# <a name="group-removefavorite"></a><span data-ttu-id="02e92-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="02e92-104">group: removeFavorite</span></span>

<span data-ttu-id="02e92-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e92-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02e92-106">Удаление группы из списка избранных групп текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="02e92-106">Remove the group from the list of the current user's favorite groups.</span></span> <span data-ttu-id="02e92-107">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="02e92-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="02e92-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02e92-108">Permissions</span></span>
<span data-ttu-id="02e92-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e92-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02e92-111">Permission type</span></span>      | <span data-ttu-id="02e92-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02e92-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02e92-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02e92-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02e92-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e92-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02e92-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02e92-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02e92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e92-116">Not supported.</span></span>    |
|<span data-ttu-id="02e92-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02e92-117">Application</span></span> | <span data-ttu-id="02e92-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e92-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02e92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02e92-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="02e92-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02e92-120">Request headers</span></span>
| <span data-ttu-id="02e92-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02e92-121">Header</span></span>       | <span data-ttu-id="02e92-122">Значение</span><span class="sxs-lookup"><span data-stu-id="02e92-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02e92-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02e92-123">Authorization</span></span>  | <span data-ttu-id="02e92-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02e92-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="02e92-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="02e92-126">Prefer</span></span> | <span data-ttu-id="02e92-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="02e92-127">return=minimal.</span></span> <span data-ttu-id="02e92-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02e92-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="02e92-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="02e92-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="02e92-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02e92-130">Request body</span></span>
<span data-ttu-id="02e92-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02e92-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02e92-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e92-132">Response</span></span>
<span data-ttu-id="02e92-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="02e92-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e92-135">Пример</span><span class="sxs-lookup"><span data-stu-id="02e92-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="02e92-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="02e92-136">Request</span></span>
<span data-ttu-id="02e92-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02e92-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02e92-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="02e92-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```
# <a name="c"></a>[<span data-ttu-id="02e92-139">C#</span><span class="sxs-lookup"><span data-stu-id="02e92-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02e92-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02e92-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02e92-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02e92-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02e92-142">Java</span><span class="sxs-lookup"><span data-stu-id="02e92-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removefavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="02e92-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e92-143">Response</span></span>
<span data-ttu-id="02e92-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="02e92-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


