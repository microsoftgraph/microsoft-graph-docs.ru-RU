---
title: 'group: addFavorite'
description: Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5878c3b0ac324592204310c80458744e4e54c446
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916392"
---
# <a name="group-addfavorite"></a><span data-ttu-id="441c7-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="441c7-104">group: addFavorite</span></span>
<span data-ttu-id="441c7-p102">Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="441c7-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="441c7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="441c7-107">Permissions</span></span>
<span data-ttu-id="441c7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="441c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="441c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="441c7-110">Permission type</span></span>      | <span data-ttu-id="441c7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="441c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="441c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="441c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="441c7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="441c7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="441c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="441c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="441c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="441c7-115">Not supported.</span></span>    |
|<span data-ttu-id="441c7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="441c7-116">Application</span></span> | <span data-ttu-id="441c7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="441c7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="441c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="441c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="441c7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="441c7-119">Request headers</span></span>
| <span data-ttu-id="441c7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="441c7-120">Header</span></span>       | <span data-ttu-id="441c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="441c7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="441c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="441c7-122">Authorization</span></span>  | <span data-ttu-id="441c7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="441c7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="441c7-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="441c7-125">Prefer</span></span> | <span data-ttu-id="441c7-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="441c7-126">return=minimal.</span></span> <span data-ttu-id="441c7-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="441c7-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="441c7-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="441c7-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="441c7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="441c7-129">Request body</span></span>
<span data-ttu-id="441c7-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="441c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="441c7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="441c7-131">Response</span></span>
<span data-ttu-id="441c7-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="441c7-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="441c7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="441c7-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="441c7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="441c7-135">Request</span></span>
<span data-ttu-id="441c7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="441c7-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="441c7-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="441c7-137">Response</span></span>
<span data-ttu-id="441c7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="441c7-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
