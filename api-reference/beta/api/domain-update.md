---
title: Обновление домена
description: Обновление свойств объекта Domain.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9099dc74de85755c0268e4eb7e96fc9b7f523a1e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963939"
---
# <a name="update-domain"></a><span data-ttu-id="a5028-103">Обновление домена</span><span class="sxs-lookup"><span data-stu-id="a5028-103">Update domain</span></span>

<span data-ttu-id="a5028-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5028-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5028-105">Обновление свойств объекта Domain.</span><span class="sxs-lookup"><span data-stu-id="a5028-105">Update the properties of domain object.</span></span>

> <span data-ttu-id="a5028-106">**Важно!** Обновлять можно только проверенные домены.</span><span class="sxs-lookup"><span data-stu-id="a5028-106">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5028-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5028-107">Permissions</span></span>

<span data-ttu-id="a5028-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5028-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5028-110">Permission type</span></span>      | <span data-ttu-id="a5028-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5028-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5028-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5028-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5028-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5028-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5028-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5028-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5028-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5028-115">Not supported.</span></span>    |
|<span data-ttu-id="a5028-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a5028-116">Application</span></span> | <span data-ttu-id="a5028-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5028-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5028-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5028-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="a5028-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="a5028-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5028-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5028-120">Request headers</span></span>

| <span data-ttu-id="a5028-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a5028-121">Name</span></span>       | <span data-ttu-id="a5028-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a5028-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a5028-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5028-123">Authorization</span></span>  | <span data-ttu-id="a5028-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5028-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5028-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5028-126">Content-Type</span></span>  | <span data-ttu-id="a5028-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a5028-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5028-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5028-128">Request body</span></span>

<span data-ttu-id="a5028-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a5028-129">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="a5028-130">Существующие свойства, не включенные в текст запроса, сохраняют свои предыдущие значения или пересчитываются в зависимости от изменений значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a5028-130">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a5028-131">Для достижения лучшей производительности включайте только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="a5028-131">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="a5028-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5028-132">Response</span></span>

<span data-ttu-id="a5028-133">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="a5028-133">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5028-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a5028-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5028-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5028-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a5028-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5028-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a5028-137">C#</span><span class="sxs-lookup"><span data-stu-id="a5028-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5028-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5028-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5028-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5028-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5028-140">Java</span><span class="sxs-lookup"><span data-stu-id="a5028-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5028-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5028-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


