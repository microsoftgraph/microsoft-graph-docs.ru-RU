---
title: Удаление соглашения
description: Удаление объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 59deacabb1ad824b6672cfc52f2280f6b693ce63
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408549"
---
# <a name="delete-agreement"></a><span data-ttu-id="1a339-103">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="1a339-103">Delete agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a339-104">Удаление объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="1a339-104">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a339-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a339-105">Permissions</span></span>
<span data-ttu-id="1a339-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a339-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a339-108">Permission type</span></span>                        | <span data-ttu-id="1a339-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a339-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a339-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a339-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a339-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a339-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="1a339-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a339-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a339-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a339-113">Not supported.</span></span> |
|<span data-ttu-id="1a339-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a339-114">Application</span></span>                            | <span data-ttu-id="1a339-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a339-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a339-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a339-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1a339-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a339-117">Request headers</span></span>
| <span data-ttu-id="1a339-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1a339-118">Name</span></span>         | <span data-ttu-id="1a339-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1a339-119">Type</span></span>        | <span data-ttu-id="1a339-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1a339-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1a339-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a339-121">Authorization</span></span> | <span data-ttu-id="1a339-122">string</span><span class="sxs-lookup"><span data-stu-id="1a339-122">string</span></span> | <span data-ttu-id="1a339-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a339-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a339-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a339-125">Request body</span></span>
<span data-ttu-id="1a339-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a339-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1a339-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a339-127">Response</span></span>
<span data-ttu-id="1a339-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a339-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a339-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1a339-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a339-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a339-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a339-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a339-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/agreements/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a339-133">C#</span><span class="sxs-lookup"><span data-stu-id="1a339-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a339-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a339-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a339-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1a339-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a339-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a339-136">Response</span></span>
><span data-ttu-id="1a339-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a339-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
