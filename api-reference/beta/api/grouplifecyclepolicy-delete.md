---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
ms.openlocfilehash: 0e291ec0d05f03153f18974ad0aad29f2a8a86d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075606"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="fbbf9-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="fbbf9-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="fbbf9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fbbf9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbbf9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbbf9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbbf9-106">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fbbf9-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbbf9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbbf9-107">Permissions</span></span>

<span data-ttu-id="fbbf9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbbf9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbbf9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbbf9-110">Permission type</span></span>      | <span data-ttu-id="fbbf9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbbf9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbbf9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbbf9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fbbf9-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbbf9-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbbf9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbbf9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbbf9-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fbbf9-115">Not supported</span></span> |
|<span data-ttu-id="fbbf9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbbf9-116">Application</span></span> | <span data-ttu-id="fbbf9-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbbf9-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbbf9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbbf9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="fbbf9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbbf9-119">Request headers</span></span>

| <span data-ttu-id="fbbf9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fbbf9-120">Name</span></span> | <span data-ttu-id="fbbf9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fbbf9-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="fbbf9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbbf9-122">Authorization</span></span> | <span data-ttu-id="fbbf9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbbf9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbbf9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbbf9-125">Content-Type</span></span>  | <span data-ttu-id="fbbf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbbf9-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbbf9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbbf9-127">Request body</span></span>
<span data-ttu-id="fbbf9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fbbf9-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fbbf9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbbf9-129">Response</span></span>

<span data-ttu-id="fbbf9-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fbbf9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbbf9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fbbf9-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fbbf9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbbf9-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="fbbf9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbbf9-134">Response</span></span>

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