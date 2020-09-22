---
title: 'securityAction: Канцелсекуритяктион'
description: Отмена операции безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 87cb0eca08e1d8c1dce81440fbaed40d12b46fa8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046953"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="317a6-103">securityAction: Канцелсекуритяктион</span><span class="sxs-lookup"><span data-stu-id="317a6-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="317a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="317a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="317a6-105">Отмена операции безопасности.</span><span class="sxs-lookup"><span data-stu-id="317a6-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="317a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="317a6-106">Permissions</span></span>

<span data-ttu-id="317a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="317a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="317a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="317a6-109">Permission type</span></span>                        | <span data-ttu-id="317a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="317a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="317a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="317a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="317a6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="317a6-112">Not supported.</span></span> |
| <span data-ttu-id="317a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="317a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="317a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="317a6-114">Not supported.</span></span> |
| <span data-ttu-id="317a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="317a6-115">Application</span></span>                            | <span data-ttu-id="317a6-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="317a6-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="317a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="317a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="317a6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="317a6-118">Request headers</span></span>

| <span data-ttu-id="317a6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="317a6-119">Name</span></span>          | <span data-ttu-id="317a6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="317a6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="317a6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="317a6-121">Authorization</span></span> | <span data-ttu-id="317a6-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="317a6-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="317a6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="317a6-123">Request body</span></span>

<span data-ttu-id="317a6-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="317a6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="317a6-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="317a6-125">Response</span></span>

<span data-ttu-id="317a6-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="317a6-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="317a6-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="317a6-128">Examples</span></span>

<span data-ttu-id="317a6-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="317a6-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="317a6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="317a6-130">Request</span></span>

<span data-ttu-id="317a6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="317a6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="317a6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="317a6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="317a6-133">C#</span><span class="sxs-lookup"><span data-stu-id="317a6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="317a6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="317a6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="317a6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="317a6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="317a6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="317a6-136">Response</span></span>

<span data-ttu-id="317a6-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="317a6-137">The following is an example of the response.</span></span>
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


