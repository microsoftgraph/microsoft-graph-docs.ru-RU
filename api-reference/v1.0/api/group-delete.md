---
title: Удаление группы
description: Удаление группы.
author: dkershaw10
ms.openlocfilehash: 6377c3d7865ebcc1ef13a649afbde083163e7048
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326280"
---
# <a name="delete-group"></a><span data-ttu-id="42a50-103">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="42a50-103">Delete group</span></span>
<span data-ttu-id="42a50-104">Удаление группы.</span><span class="sxs-lookup"><span data-stu-id="42a50-104">Delete group.</span></span>

## <a name="permissions"></a><span data-ttu-id="42a50-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42a50-105">Permissions</span></span>
<span data-ttu-id="42a50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42a50-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42a50-108">Permission type</span></span>      | <span data-ttu-id="42a50-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42a50-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42a50-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42a50-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42a50-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a50-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42a50-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42a50-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42a50-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a50-113">Not supported.</span></span>    |
|<span data-ttu-id="42a50-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42a50-114">Application</span></span> | <span data-ttu-id="42a50-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a50-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42a50-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42a50-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="42a50-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42a50-117">Request headers</span></span>
| <span data-ttu-id="42a50-118">Имя</span><span class="sxs-lookup"><span data-stu-id="42a50-118">Name</span></span>       | <span data-ttu-id="42a50-119">Тип</span><span class="sxs-lookup"><span data-stu-id="42a50-119">Type</span></span> | <span data-ttu-id="42a50-120">Описание</span><span class="sxs-lookup"><span data-stu-id="42a50-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42a50-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="42a50-121">Authorization</span></span>  | <span data-ttu-id="42a50-122">string</span><span class="sxs-lookup"><span data-stu-id="42a50-122">string</span></span>  | <span data-ttu-id="42a50-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42a50-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42a50-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42a50-125">Request body</span></span>
<span data-ttu-id="42a50-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42a50-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42a50-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a50-127">Response</span></span>
<span data-ttu-id="42a50-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="42a50-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42a50-130">Пример</span><span class="sxs-lookup"><span data-stu-id="42a50-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="42a50-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="42a50-131">Request</span></span>
<span data-ttu-id="42a50-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42a50-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="42a50-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="42a50-133">Response</span></span>
<span data-ttu-id="42a50-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42a50-134">The following is an example of the response.</span></span> 
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