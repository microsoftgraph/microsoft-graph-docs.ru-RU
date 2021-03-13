---
title: Удаление соглашения
description: Удаление объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 00429565e3b23547573653186fdea00b6aea760c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774028"
---
# <a name="delete-agreement"></a><span data-ttu-id="9e25f-103">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="9e25f-103">Delete agreement</span></span>

<span data-ttu-id="9e25f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e25f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e25f-105">Удаление объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="9e25f-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e25f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e25f-106">Permissions</span></span>
<span data-ttu-id="9e25f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e25f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e25f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e25f-109">Permission type</span></span>                        | <span data-ttu-id="9e25f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e25f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e25f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e25f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e25f-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e25f-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="9e25f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e25f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e25f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e25f-114">Not supported.</span></span> |
|<span data-ttu-id="9e25f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e25f-115">Application</span></span>                            | <span data-ttu-id="9e25f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e25f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e25f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e25f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9e25f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e25f-118">Request headers</span></span>
| <span data-ttu-id="9e25f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9e25f-119">Name</span></span>         | <span data-ttu-id="9e25f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9e25f-120">Type</span></span>        | <span data-ttu-id="9e25f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9e25f-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9e25f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e25f-122">Authorization</span></span> | <span data-ttu-id="9e25f-123">string</span><span class="sxs-lookup"><span data-stu-id="9e25f-123">string</span></span> | <span data-ttu-id="9e25f-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e25f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e25f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e25f-126">Request body</span></span>
<span data-ttu-id="9e25f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e25f-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9e25f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e25f-128">Response</span></span>
<span data-ttu-id="9e25f-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9e25f-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e25f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e25f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e25f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e25f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9e25f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e25f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
```
# <a name="c"></a>[<span data-ttu-id="9e25f-134">C#</span><span class="sxs-lookup"><span data-stu-id="9e25f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e25f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e25f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e25f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e25f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e25f-137">Java</span><span class="sxs-lookup"><span data-stu-id="9e25f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e25f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e25f-138">Response</span></span>
><span data-ttu-id="9e25f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e25f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


