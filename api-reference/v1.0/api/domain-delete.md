---
title: Удаление домена
description: Удаление домена из клиента.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: abe6ca111236ba4c723882b7dcf63df630c22c28
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33617015"
---
# <a name="delete-domain"></a><span data-ttu-id="ab536-103">Удаление домена</span><span class="sxs-lookup"><span data-stu-id="ab536-103">Delete domain</span></span>

<span data-ttu-id="ab536-104">Удаление домена из клиента.</span><span class="sxs-lookup"><span data-stu-id="ab536-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="ab536-105">**Важно!**</span><span class="sxs-lookup"><span data-stu-id="ab536-105">**Important:**</span></span>
> - <span data-ttu-id="ab536-106">Вам не удастся восстановить удаленные домены.</span><span class="sxs-lookup"><span data-stu-id="ab536-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="ab536-p101">Вам не удастся удалить домен, если какие-либо ресурсы или объекты все еще зависят от него. Вы можете найти все зависимые ресурсы с помощью API [перечисления domainNameReferences](domain-list-domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="ab536-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab536-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab536-109">Permissions</span></span>

<span data-ttu-id="ab536-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab536-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ab536-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab536-112">Permission type</span></span>      | <span data-ttu-id="ab536-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab536-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab536-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab536-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ab536-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab536-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab536-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab536-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab536-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab536-117">Not supported.</span></span>    |
|<span data-ttu-id="ab536-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab536-118">Application</span></span> | <span data-ttu-id="ab536-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab536-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab536-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab536-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="ab536-121">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="ab536-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab536-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab536-122">Request headers</span></span>

| <span data-ttu-id="ab536-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ab536-123">Name</span></span>       | <span data-ttu-id="ab536-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ab536-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab536-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab536-125">Authorization</span></span>  | <span data-ttu-id="ab536-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab536-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab536-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab536-128">Content-Type</span></span>  | <span data-ttu-id="ab536-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ab536-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab536-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab536-130">Request body</span></span>

<span data-ttu-id="ab536-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab536-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab536-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab536-132">Response</span></span>

<span data-ttu-id="ab536-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Он не возвращает тело отклика.</span><span class="sxs-lookup"><span data-stu-id="ab536-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab536-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ab536-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab536-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab536-136">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="ab536-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab536-137">Response</span></span>

<span data-ttu-id="ab536-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab536-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ab536-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ab536-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ab536-141">Языках</span><span class="sxs-lookup"><span data-stu-id="ab536-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab536-142">Язык</span><span class="sxs-lookup"><span data-stu-id="ab536-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
