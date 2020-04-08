---
title: Обновление домена
description: Обновление свойств объекта Domain.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6c39f488b3d41c099d996023617d726be09a9cdf
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43179845"
---
# <a name="update-domain"></a><span data-ttu-id="4a989-103">Обновление домена</span><span class="sxs-lookup"><span data-stu-id="4a989-103">Update domain</span></span>

<span data-ttu-id="4a989-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a989-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a989-105">Обновление свойств объекта Domain.</span><span class="sxs-lookup"><span data-stu-id="4a989-105">Update the properties of domain object.</span></span>

> <span data-ttu-id="4a989-106">**Важно!** Обновлять можно только проверенные домены.</span><span class="sxs-lookup"><span data-stu-id="4a989-106">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a989-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a989-107">Permissions</span></span>

<span data-ttu-id="4a989-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a989-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a989-110">Permission type</span></span>      | <span data-ttu-id="4a989-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a989-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a989-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a989-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a989-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a989-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a989-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a989-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a989-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a989-115">Not supported.</span></span>    |
|<span data-ttu-id="4a989-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a989-116">Application</span></span> | <span data-ttu-id="4a989-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a989-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a989-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a989-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="4a989-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="4a989-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a989-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a989-120">Request headers</span></span>

| <span data-ttu-id="4a989-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4a989-121">Name</span></span>       | <span data-ttu-id="4a989-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4a989-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4a989-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a989-123">Authorization</span></span>  | <span data-ttu-id="4a989-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a989-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a989-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a989-126">Content-Type</span></span>  | <span data-ttu-id="4a989-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4a989-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a989-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a989-128">Request body</span></span>

<span data-ttu-id="4a989-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4a989-129">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="4a989-130">Существующие свойства, не включенные в текст запроса, сохраняют свои предыдущие значения или пересчитываются в зависимости от изменений значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4a989-130">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4a989-131">Для достижения лучшей производительности включайте только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="4a989-131">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="4a989-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a989-132">Response</span></span>

<span data-ttu-id="4a989-133">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="4a989-133">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a989-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4a989-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a989-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a989-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4a989-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a989-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4a989-137">C#</span><span class="sxs-lookup"><span data-stu-id="4a989-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a989-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a989-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a989-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a989-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4a989-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a989-140">Response</span></span>

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
