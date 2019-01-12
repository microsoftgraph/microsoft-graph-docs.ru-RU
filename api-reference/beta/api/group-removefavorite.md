---
title: 'group: removeFavorite'
description: Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9ed755add4771b062d004aaa35c55b9afd23a390
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951021"
---
# <a name="group-removefavorite"></a><span data-ttu-id="5c8b7-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="5c8b7-104">group: removeFavorite</span></span>

> <span data-ttu-id="5c8b7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c8b7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c8b7-p103">Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-p103">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c8b7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c8b7-109">Permissions</span></span>
<span data-ttu-id="5c8b7-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c8b7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c8b7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c8b7-112">Permission type</span></span>      | <span data-ttu-id="5c8b7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c8b7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c8b7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c8b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5c8b7-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c8b7-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c8b7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c8b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c8b7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-117">Not supported.</span></span>    |
|<span data-ttu-id="5c8b7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c8b7-118">Application</span></span> | <span data-ttu-id="5c8b7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c8b7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c8b7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="5c8b7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c8b7-121">Request headers</span></span>
| <span data-ttu-id="5c8b7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c8b7-122">Header</span></span>       | <span data-ttu-id="5c8b7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5c8b7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c8b7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c8b7-124">Authorization</span></span>  | <span data-ttu-id="5c8b7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5c8b7-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="5c8b7-127">Prefer</span></span> | <span data-ttu-id="5c8b7-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-128">return=minimal.</span></span> <span data-ttu-id="5c8b7-129">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="5c8b7-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="5c8b7-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c8b7-131">Request body</span></span>
<span data-ttu-id="5c8b7-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c8b7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c8b7-133">Response</span></span>
<span data-ttu-id="5c8b7-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c8b7-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5c8b7-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5c8b7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c8b7-137">Request</span></span>
<span data-ttu-id="5c8b7-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="5c8b7-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c8b7-139">Response</span></span>
<span data-ttu-id="5c8b7-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5c8b7-140">The following is an example of the response.</span></span>
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
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
