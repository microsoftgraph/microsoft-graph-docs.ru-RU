---
title: Обновление домена
description: Обновление свойств объекта домена.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ee201a5dbd60e68c9e3e53e5c7dba340fe1ef06b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441958"
---
# <a name="update-domain"></a><span data-ttu-id="f5637-103">Обновление домена</span><span class="sxs-lookup"><span data-stu-id="f5637-103">Update domain</span></span>

<span data-ttu-id="f5637-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5637-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5637-105">Обновление свойств объекта домена.</span><span class="sxs-lookup"><span data-stu-id="f5637-105">Update the properties of domain object.</span></span>

> <span data-ttu-id="f5637-106">**Важно:** Обновить можно только проверенные домены.</span><span class="sxs-lookup"><span data-stu-id="f5637-106">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5637-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5637-107">Permissions</span></span>

<span data-ttu-id="f5637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f5637-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5637-110">Permission type</span></span>      | <span data-ttu-id="f5637-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5637-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5637-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5637-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5637-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5637-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f5637-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5637-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5637-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5637-115">Not supported.</span></span>    |
|<span data-ttu-id="f5637-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5637-116">Application</span></span> | <span data-ttu-id="f5637-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5637-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5637-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5637-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="f5637-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="f5637-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5637-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5637-120">Request headers</span></span>

| <span data-ttu-id="f5637-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f5637-121">Name</span></span>       | <span data-ttu-id="f5637-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f5637-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f5637-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5637-123">Authorization</span></span>  | <span data-ttu-id="f5637-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5637-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5637-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5637-126">Content-Type</span></span>  | <span data-ttu-id="f5637-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f5637-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5637-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5637-128">Request body</span></span>

<span data-ttu-id="f5637-129">В теле запроса укажи значения для обновляемой области.</span><span class="sxs-lookup"><span data-stu-id="f5637-129">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="f5637-130">Существующие свойства, не включенные в тело запроса, будут поддерживать прежние значения или пересчитываться на основе изменений в других значениях свойств.</span><span class="sxs-lookup"><span data-stu-id="f5637-130">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f5637-131">Для лучшей производительности включаем только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="f5637-131">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="f5637-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5637-132">Response</span></span>

<span data-ttu-id="f5637-133">В случае успешной работы этот метод возвращает код `204 No Content` ответа и не возвращает текст ответа.</span><span class="sxs-lookup"><span data-stu-id="f5637-133">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5637-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f5637-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5637-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5637-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f5637-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5637-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="f5637-137">C#</span><span class="sxs-lookup"><span data-stu-id="f5637-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5637-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5637-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5637-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5637-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5637-140">Java</span><span class="sxs-lookup"><span data-stu-id="f5637-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f5637-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5637-141">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

