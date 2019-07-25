---
title: 'securityAction: Канцелсекуритяктион'
description: Отмена операции безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 953fa3ce38597c84f3f87f71f5b6746ad86e495e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870316"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="305c2-103">securityAction: Канцелсекуритяктион</span><span class="sxs-lookup"><span data-stu-id="305c2-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="305c2-104">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="305c2-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="305c2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="305c2-105">Permissions</span></span>

<span data-ttu-id="305c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="305c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="305c2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="305c2-108">Permission type</span></span>                        | <span data-ttu-id="305c2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="305c2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="305c2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="305c2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="305c2-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="305c2-111">Not supported.</span></span> |
| <span data-ttu-id="305c2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="305c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="305c2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="305c2-113">Not supported.</span></span> |
| <span data-ttu-id="305c2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="305c2-114">Application</span></span>                            | <span data-ttu-id="305c2-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="305c2-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="305c2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="305c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="305c2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="305c2-117">Request headers</span></span>

| <span data-ttu-id="305c2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="305c2-118">Name</span></span>          | <span data-ttu-id="305c2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="305c2-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="305c2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="305c2-120">Authorization</span></span> | <span data-ttu-id="305c2-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="305c2-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="305c2-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="305c2-122">Request body</span></span>

<span data-ttu-id="305c2-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="305c2-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="305c2-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="305c2-124">Response</span></span>

<span data-ttu-id="305c2-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="305c2-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="305c2-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="305c2-127">Examples</span></span>

<span data-ttu-id="305c2-128">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="305c2-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="305c2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="305c2-129">Request</span></span>

<span data-ttu-id="305c2-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="305c2-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="305c2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="305c2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="305c2-132">C#</span><span class="sxs-lookup"><span data-stu-id="305c2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="305c2-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="305c2-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="305c2-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="305c2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="305c2-135">Java</span><span class="sxs-lookup"><span data-stu-id="305c2-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securityaction-cancelsecurityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="305c2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="305c2-136">Response</span></span>

<span data-ttu-id="305c2-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="305c2-137">The following is an example of the response.</span></span>
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
