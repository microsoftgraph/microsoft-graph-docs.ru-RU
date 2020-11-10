---
title: 'securityAction: Канцелсекуритяктион'
description: Отмена операции безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: a12f902c3f2eeed89c40497c49d9bb1a78fe6123
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976716"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="a3537-103">securityAction: Канцелсекуритяктион</span><span class="sxs-lookup"><span data-stu-id="a3537-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="a3537-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3537-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3537-105">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="a3537-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3537-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3537-106">Permissions</span></span>

<span data-ttu-id="a3537-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3537-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3537-109">Permission type</span></span>                        | <span data-ttu-id="a3537-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3537-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a3537-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3537-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3537-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3537-112">Not supported.</span></span> |
| <span data-ttu-id="a3537-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3537-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3537-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3537-114">Not supported.</span></span> |
| <span data-ttu-id="a3537-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a3537-115">Application</span></span>                            | <span data-ttu-id="a3537-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3537-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3537-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3537-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="a3537-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3537-118">Request headers</span></span>

| <span data-ttu-id="a3537-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a3537-119">Name</span></span>          | <span data-ttu-id="a3537-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3537-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a3537-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3537-121">Authorization</span></span> | <span data-ttu-id="a3537-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a3537-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3537-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3537-123">Request body</span></span>

<span data-ttu-id="a3537-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3537-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3537-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3537-125">Response</span></span>

<span data-ttu-id="a3537-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a3537-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3537-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a3537-128">Examples</span></span>

<span data-ttu-id="a3537-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a3537-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a3537-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3537-130">Request</span></span>

<span data-ttu-id="a3537-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3537-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3537-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3537-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="a3537-133">C#</span><span class="sxs-lookup"><span data-stu-id="a3537-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3537-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3537-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3537-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3537-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3537-136">Java</span><span class="sxs-lookup"><span data-stu-id="a3537-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securityaction-cancelsecurityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3537-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3537-137">Response</span></span>

<span data-ttu-id="a3537-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a3537-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


