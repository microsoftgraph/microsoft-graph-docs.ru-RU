---
title: 'securityAction: cancelSecurityAction'
description: Отмена операции безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 41cec1694baa05b67791a000215f44c6cfd8c859
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787235"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="beedf-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="beedf-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="beedf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beedf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beedf-105">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="beedf-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="beedf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="beedf-106">Permissions</span></span>

<span data-ttu-id="beedf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beedf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="beedf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beedf-109">Permission type</span></span>                        | <span data-ttu-id="beedf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="beedf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="beedf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beedf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="beedf-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beedf-112">Not supported.</span></span> |
| <span data-ttu-id="beedf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beedf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beedf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beedf-114">Not supported.</span></span> |
| <span data-ttu-id="beedf-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="beedf-115">Application</span></span>                            | <span data-ttu-id="beedf-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beedf-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="beedf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beedf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="beedf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beedf-118">Request headers</span></span>

| <span data-ttu-id="beedf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="beedf-119">Name</span></span>          | <span data-ttu-id="beedf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="beedf-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="beedf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beedf-121">Authorization</span></span> | <span data-ttu-id="beedf-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="beedf-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="beedf-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beedf-123">Request body</span></span>

<span data-ttu-id="beedf-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="beedf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beedf-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="beedf-125">Response</span></span>

<span data-ttu-id="beedf-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="beedf-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="beedf-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="beedf-128">Examples</span></span>

<span data-ttu-id="beedf-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="beedf-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="beedf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="beedf-130">Request</span></span>

<span data-ttu-id="beedf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beedf-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="beedf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="beedf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="beedf-133">C#</span><span class="sxs-lookup"><span data-stu-id="beedf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="beedf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="beedf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="beedf-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="beedf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="beedf-136">Java</span><span class="sxs-lookup"><span data-stu-id="beedf-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securityaction-cancelsecurityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="beedf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="beedf-137">Response</span></span>

<span data-ttu-id="beedf-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="beedf-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


