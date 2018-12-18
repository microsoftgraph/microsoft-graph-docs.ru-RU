---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: lleonard-msft
ms.openlocfilehash: c2b0f8896ca2cc13ebb9f53900638875ade365bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302417"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="85a81-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="85a81-103">Remove directory role member</span></span>

> <span data-ttu-id="85a81-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85a81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85a81-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85a81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85a81-106">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="85a81-106">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="85a81-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85a81-107">Permissions</span></span>

<span data-ttu-id="85a81-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85a81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="85a81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85a81-110">Permission type</span></span>      | <span data-ttu-id="85a81-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85a81-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85a81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85a81-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85a81-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85a81-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="85a81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85a81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85a81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85a81-115">Not supported.</span></span>    |
|<span data-ttu-id="85a81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85a81-116">Application</span></span> | <span data-ttu-id="85a81-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85a81-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85a81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85a81-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="85a81-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85a81-119">Request headers</span></span>

| <span data-ttu-id="85a81-120">Имя</span><span class="sxs-lookup"><span data-stu-id="85a81-120">Name</span></span>       | <span data-ttu-id="85a81-121">Тип</span><span class="sxs-lookup"><span data-stu-id="85a81-121">Type</span></span> | <span data-ttu-id="85a81-122">Описание</span><span class="sxs-lookup"><span data-stu-id="85a81-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="85a81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85a81-123">Authorization</span></span>  | <span data-ttu-id="85a81-124">string</span><span class="sxs-lookup"><span data-stu-id="85a81-124">string</span></span>  | <span data-ttu-id="85a81-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85a81-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85a81-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85a81-127">Request body</span></span>

<span data-ttu-id="85a81-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85a81-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85a81-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="85a81-129">Response</span></span>

<span data-ttu-id="85a81-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="85a81-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85a81-132">Пример</span><span class="sxs-lookup"><span data-stu-id="85a81-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85a81-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="85a81-133">Request</span></span>

<span data-ttu-id="85a81-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85a81-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="85a81-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="85a81-135">Response</span></span>

<span data-ttu-id="85a81-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85a81-136">Here is an example of the response.</span></span> 
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