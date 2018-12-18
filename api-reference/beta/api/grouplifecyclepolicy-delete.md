---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: dkershaw10
ms.openlocfilehash: 41c679a9fa2a55a0137d1197f08515e64750d4dc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361966"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="5411d-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="5411d-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="5411d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5411d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5411d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5411d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5411d-106">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5411d-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5411d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5411d-107">Permissions</span></span>

<span data-ttu-id="5411d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5411d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5411d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5411d-110">Permission type</span></span>      | <span data-ttu-id="5411d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5411d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5411d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5411d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5411d-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5411d-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="5411d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5411d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5411d-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5411d-115">Not supported</span></span> |
|<span data-ttu-id="5411d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5411d-116">Application</span></span> | <span data-ttu-id="5411d-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5411d-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5411d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5411d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="5411d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5411d-119">Request headers</span></span>

| <span data-ttu-id="5411d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5411d-120">Name</span></span> | <span data-ttu-id="5411d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5411d-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5411d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5411d-122">Authorization</span></span> | <span data-ttu-id="5411d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5411d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5411d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5411d-125">Content-Type</span></span>  | <span data-ttu-id="5411d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5411d-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5411d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5411d-127">Request body</span></span>
<span data-ttu-id="5411d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5411d-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5411d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5411d-129">Response</span></span>

<span data-ttu-id="5411d-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5411d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5411d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5411d-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5411d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5411d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="5411d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5411d-134">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->