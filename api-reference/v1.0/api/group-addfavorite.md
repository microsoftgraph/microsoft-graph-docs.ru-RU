---
title: 'group: addFavorite'
description: Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5878c3b0ac324592204310c80458744e4e54c446
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524164"
---
# <a name="group-addfavorite"></a><span data-ttu-id="2c585-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="2c585-104">group: addFavorite</span></span>
<span data-ttu-id="2c585-p102">Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="2c585-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c585-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c585-107">Permissions</span></span>
<span data-ttu-id="2c585-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c585-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c585-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c585-110">Permission type</span></span>      | <span data-ttu-id="2c585-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c585-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c585-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c585-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c585-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c585-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c585-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c585-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c585-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c585-115">Not supported.</span></span>    |
|<span data-ttu-id="2c585-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c585-116">Application</span></span> | <span data-ttu-id="2c585-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c585-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c585-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c585-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="2c585-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c585-119">Request headers</span></span>
| <span data-ttu-id="2c585-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c585-120">Header</span></span>       | <span data-ttu-id="2c585-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2c585-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c585-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c585-122">Authorization</span></span>  | <span data-ttu-id="2c585-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c585-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c585-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="2c585-125">Prefer</span></span> | <span data-ttu-id="2c585-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="2c585-126">return=minimal.</span></span> <span data-ttu-id="2c585-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c585-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="2c585-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2c585-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c585-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2c585-129">Request body</span></span>
<span data-ttu-id="2c585-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2c585-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c585-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c585-131">Response</span></span>
<span data-ttu-id="2c585-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2c585-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c585-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2c585-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2c585-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c585-135">Request</span></span>
<span data-ttu-id="2c585-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c585-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="2c585-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c585-137">Response</span></span>
<span data-ttu-id="2c585-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c585-138">The following is an example of the response.</span></span>
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
