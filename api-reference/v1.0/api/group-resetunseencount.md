---
title: 'group: resetUnseenCount'
description: Сброс unseenCount всех записей, которые текущий пользователь не просматривал со времени своего предыдущего посещения. Поддерживается только для групп Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0c875615fb9650ecafafd503d37e88b0473fd482
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521210"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="901f0-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="901f0-104">group: resetUnseenCount</span></span>
<span data-ttu-id="901f0-p102">Сброс unseenCount всех записей, которые текущий пользователь не просматривал со времени своего предыдущего посещения. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="901f0-p102">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="901f0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="901f0-107">Permissions</span></span>
<span data-ttu-id="901f0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="901f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="901f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="901f0-110">Permission type</span></span>      | <span data-ttu-id="901f0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="901f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="901f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="901f0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="901f0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901f0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="901f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="901f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="901f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="901f0-115">Not supported.</span></span>    |
|<span data-ttu-id="901f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="901f0-116">Application</span></span> | <span data-ttu-id="901f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="901f0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="901f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="901f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="901f0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="901f0-119">Request headers</span></span>
| <span data-ttu-id="901f0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="901f0-120">Header</span></span>       | <span data-ttu-id="901f0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="901f0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="901f0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="901f0-122">Authorization</span></span>  | <span data-ttu-id="901f0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="901f0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="901f0-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="901f0-125">Prefer</span></span> | <span data-ttu-id="901f0-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="901f0-126">return=minimal.</span></span> <span data-ttu-id="901f0-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="901f0-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="901f0-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="901f0-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="901f0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="901f0-129">Request body</span></span>
<span data-ttu-id="901f0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="901f0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="901f0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="901f0-131">Response</span></span>
<span data-ttu-id="901f0-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="901f0-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="901f0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="901f0-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="901f0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="901f0-135">Request</span></span>
<span data-ttu-id="901f0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="901f0-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="901f0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="901f0-137">Response</span></span>
<span data-ttu-id="901f0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="901f0-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
