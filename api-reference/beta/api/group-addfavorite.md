---
title: 'group: addFavorite'
description: Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 936b2e8182cae8847d2043b0c8984fb3e6e8ba1f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984481"
---
# <a name="group-addfavorite"></a><span data-ttu-id="a2300-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="a2300-104">group: addFavorite</span></span>

> <span data-ttu-id="a2300-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2300-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2300-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2300-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2300-p103">Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="a2300-p103">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2300-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2300-109">Permissions</span></span>
<span data-ttu-id="a2300-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2300-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2300-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2300-112">Permission type</span></span>      | <span data-ttu-id="a2300-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2300-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2300-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2300-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a2300-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2300-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2300-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2300-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2300-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2300-117">Not supported.</span></span>    |
|<span data-ttu-id="a2300-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2300-118">Application</span></span> | <span data-ttu-id="a2300-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2300-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2300-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2300-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="a2300-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2300-121">Request headers</span></span>
| <span data-ttu-id="a2300-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2300-122">Header</span></span>       | <span data-ttu-id="a2300-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a2300-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2300-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2300-124">Authorization</span></span>  | <span data-ttu-id="a2300-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2300-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a2300-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="a2300-127">Prefer</span></span> | <span data-ttu-id="a2300-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="a2300-128">return=minimal.</span></span> <span data-ttu-id="a2300-129">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a2300-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="a2300-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a2300-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="a2300-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2300-131">Request body</span></span>
<span data-ttu-id="a2300-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2300-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2300-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2300-133">Response</span></span>
<span data-ttu-id="a2300-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a2300-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2300-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a2300-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a2300-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2300-137">Request</span></span>
<span data-ttu-id="a2300-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2300-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="a2300-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2300-139">Response</span></span>
<span data-ttu-id="a2300-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a2300-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
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
