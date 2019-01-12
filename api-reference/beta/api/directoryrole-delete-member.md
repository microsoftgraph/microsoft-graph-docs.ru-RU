---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0c218351d9c8e556220630f150f5e43592c626f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956144"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="fd6ed-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="fd6ed-103">Remove directory role member</span></span>

> <span data-ttu-id="fd6ed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd6ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd6ed-106">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-106">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd6ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd6ed-107">Permissions</span></span>

<span data-ttu-id="fd6ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd6ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fd6ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd6ed-110">Permission type</span></span>      | <span data-ttu-id="fd6ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd6ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd6ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd6ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd6ed-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd6ed-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd6ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd6ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd6ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-115">Not supported.</span></span>    |
|<span data-ttu-id="fd6ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd6ed-116">Application</span></span> | <span data-ttu-id="fd6ed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd6ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd6ed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fd6ed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd6ed-119">Request headers</span></span>

| <span data-ttu-id="fd6ed-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fd6ed-120">Name</span></span>       | <span data-ttu-id="fd6ed-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fd6ed-121">Type</span></span> | <span data-ttu-id="fd6ed-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fd6ed-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd6ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd6ed-123">Authorization</span></span>  | <span data-ttu-id="fd6ed-124">string</span><span class="sxs-lookup"><span data-stu-id="fd6ed-124">string</span></span>  | <span data-ttu-id="fd6ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd6ed-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd6ed-127">Request body</span></span>

<span data-ttu-id="fd6ed-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd6ed-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd6ed-129">Response</span></span>

<span data-ttu-id="fd6ed-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd6ed-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fd6ed-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fd6ed-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd6ed-133">Request</span></span>

<span data-ttu-id="fd6ed-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="fd6ed-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd6ed-135">Response</span></span>

<span data-ttu-id="fd6ed-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd6ed-136">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
