---
title: Удаление группы
description: Удаление группы.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b9d2e9cbe3a86906c815178b570cd6d7980ac89e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808311"
---
# <a name="delete-group"></a><span data-ttu-id="7cc47-103">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="7cc47-103">Delete group</span></span>
<span data-ttu-id="7cc47-104">Удаление группы.</span><span class="sxs-lookup"><span data-stu-id="7cc47-104">Delete group.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cc47-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cc47-105">Permissions</span></span>
<span data-ttu-id="7cc47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cc47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cc47-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cc47-108">Permission type</span></span>      | <span data-ttu-id="7cc47-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cc47-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cc47-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cc47-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7cc47-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cc47-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7cc47-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cc47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cc47-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cc47-113">Not supported.</span></span>    |
|<span data-ttu-id="7cc47-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cc47-114">Application</span></span> | <span data-ttu-id="7cc47-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cc47-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cc47-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cc47-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7cc47-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cc47-117">Request headers</span></span>
| <span data-ttu-id="7cc47-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7cc47-118">Name</span></span>       | <span data-ttu-id="7cc47-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7cc47-119">Type</span></span> | <span data-ttu-id="7cc47-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7cc47-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7cc47-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cc47-121">Authorization</span></span>  | <span data-ttu-id="7cc47-122">string</span><span class="sxs-lookup"><span data-stu-id="7cc47-122">string</span></span>  | <span data-ttu-id="7cc47-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cc47-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cc47-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7cc47-125">Request body</span></span>
<span data-ttu-id="7cc47-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7cc47-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cc47-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cc47-127">Response</span></span>
<span data-ttu-id="7cc47-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7cc47-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cc47-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7cc47-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7cc47-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cc47-131">Request</span></span>
<span data-ttu-id="7cc47-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cc47-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="7cc47-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cc47-133">Response</span></span>
<span data-ttu-id="7cc47-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7cc47-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
