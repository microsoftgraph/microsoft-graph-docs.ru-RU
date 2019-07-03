---
title: Обновление домена
description: Обновление свойств объекта Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3f887fb4089efd78f0cee4c21eb83c547d0f0385
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436657"
---
# <a name="update-domain"></a><span data-ttu-id="9a64c-103">Обновление домена</span><span class="sxs-lookup"><span data-stu-id="9a64c-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a64c-104">Обновление свойств объекта Domain.</span><span class="sxs-lookup"><span data-stu-id="9a64c-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="9a64c-105">**Важно!** Обновлять можно только проверенные домены.</span><span class="sxs-lookup"><span data-stu-id="9a64c-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a64c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a64c-106">Permissions</span></span>

<span data-ttu-id="9a64c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a64c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9a64c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a64c-109">Permission type</span></span>      | <span data-ttu-id="9a64c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a64c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a64c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a64c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a64c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a64c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a64c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a64c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a64c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a64c-114">Not supported.</span></span>    |
|<span data-ttu-id="9a64c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a64c-115">Application</span></span> | <span data-ttu-id="9a64c-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a64c-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a64c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a64c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="9a64c-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="9a64c-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a64c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a64c-119">Request headers</span></span>

| <span data-ttu-id="9a64c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9a64c-120">Name</span></span>       | <span data-ttu-id="9a64c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9a64c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a64c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a64c-122">Authorization</span></span>  | <span data-ttu-id="9a64c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a64c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a64c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a64c-125">Content-Type</span></span>  | <span data-ttu-id="9a64c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a64c-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a64c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a64c-127">Request body</span></span>

<span data-ttu-id="9a64c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9a64c-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="9a64c-129">Существующие свойства, не включенные в текст запроса, сохраняют свои предыдущие значения или пересчитываются в зависимости от изменений значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9a64c-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9a64c-130">Для достижения лучшей производительности включайте только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="9a64c-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="9a64c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a64c-131">Response</span></span>

<span data-ttu-id="9a64c-132">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="9a64c-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a64c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9a64c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a64c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a64c-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9a64c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a64c-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a64c-136">C#</span><span class="sxs-lookup"><span data-stu-id="9a64c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a64c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a64c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a64c-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9a64c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9a64c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a64c-139">Response</span></span>

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
