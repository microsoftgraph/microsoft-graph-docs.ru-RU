---
title: Удаление приложения
description: Приложение удаляется.
author: lleonard-msft
ms.openlocfilehash: e19ca94be2d8599f250908ab2aaa33d64b513b8d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343500"
---
# <a name="delete-application"></a><span data-ttu-id="2feae-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="2feae-103">Delete application</span></span>

> <span data-ttu-id="2feae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2feae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2feae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2feae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2feae-106">Приложение удаляется.</span><span class="sxs-lookup"><span data-stu-id="2feae-106">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="2feae-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2feae-107">Permissions</span></span>
<span data-ttu-id="2feae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2feae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2feae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2feae-110">Permission type</span></span>      | <span data-ttu-id="2feae-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2feae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2feae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2feae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2feae-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2feae-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2feae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2feae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2feae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2feae-115">Not supported.</span></span>    |
|<span data-ttu-id="2feae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2feae-116">Application</span></span> | <span data-ttu-id="2feae-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2feae-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2feae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2feae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2feae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2feae-119">Request headers</span></span>
| <span data-ttu-id="2feae-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2feae-120">Name</span></span>       | <span data-ttu-id="2feae-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2feae-121">Type</span></span> | <span data-ttu-id="2feae-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2feae-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2feae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2feae-123">Authorization</span></span>  | <span data-ttu-id="2feae-124">string</span><span class="sxs-lookup"><span data-stu-id="2feae-124">string</span></span>  | <span data-ttu-id="2feae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2feae-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2feae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2feae-127">Request body</span></span>
<span data-ttu-id="2feae-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2feae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2feae-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2feae-129">Response</span></span>

<span data-ttu-id="2feae-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2feae-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2feae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2feae-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2feae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2feae-133">Request</span></span>
<span data-ttu-id="2feae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2feae-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="2feae-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="2feae-135">Response</span></span>
<span data-ttu-id="2feae-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2feae-136">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->