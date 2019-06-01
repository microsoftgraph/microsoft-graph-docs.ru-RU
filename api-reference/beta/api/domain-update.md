---
title: Обновление домена
description: Обновление свойств объекта Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5c32aff2d4f2de948eb3f1a08cc08e2a1ff5a61
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655700"
---
# <a name="update-domain"></a><span data-ttu-id="629cc-103">Обновление домена</span><span class="sxs-lookup"><span data-stu-id="629cc-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="629cc-104">Обновление свойств объекта Domain.</span><span class="sxs-lookup"><span data-stu-id="629cc-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="629cc-105">**Важно!** Обновлять можно только проверенные домены.</span><span class="sxs-lookup"><span data-stu-id="629cc-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="629cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="629cc-106">Permissions</span></span>

<span data-ttu-id="629cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="629cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="629cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="629cc-109">Permission type</span></span>      | <span data-ttu-id="629cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="629cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="629cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="629cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="629cc-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="629cc-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="629cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="629cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="629cc-114">Not supported.</span></span>    |
|<span data-ttu-id="629cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="629cc-115">Application</span></span> | <span data-ttu-id="629cc-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629cc-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="629cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="629cc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="629cc-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="629cc-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="629cc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="629cc-119">Request headers</span></span>

| <span data-ttu-id="629cc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="629cc-120">Name</span></span>       | <span data-ttu-id="629cc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="629cc-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="629cc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="629cc-122">Authorization</span></span>  | <span data-ttu-id="629cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="629cc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="629cc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="629cc-125">Content-Type</span></span>  | <span data-ttu-id="629cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="629cc-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="629cc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="629cc-127">Request body</span></span>

<span data-ttu-id="629cc-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="629cc-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="629cc-129">Существующие свойства, не включенные в текст запроса, сохраняют свои предыдущие значения или пересчитываются в зависимости от изменений значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="629cc-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="629cc-130">Для достижения лучшей производительности включайте только измененные значения.</span><span class="sxs-lookup"><span data-stu-id="629cc-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="629cc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="629cc-131">Response</span></span>

<span data-ttu-id="629cc-132">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="629cc-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="629cc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="629cc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="629cc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="629cc-134">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="629cc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="629cc-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="629cc-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="629cc-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="629cc-137">C#</span><span class="sxs-lookup"><span data-stu-id="629cc-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="629cc-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="629cc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
