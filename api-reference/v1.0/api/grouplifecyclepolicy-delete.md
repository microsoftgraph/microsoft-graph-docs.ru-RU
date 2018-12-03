---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
ms.openlocfilehash: af154d2ff5e7b61a245f3b99d22f10d26f0204fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028125"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="620a4-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="620a4-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="620a4-104">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="620a4-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="620a4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="620a4-105">Permissions</span></span>

<span data-ttu-id="620a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="620a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="620a4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="620a4-108">Permission type</span></span>      | <span data-ttu-id="620a4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="620a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="620a4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="620a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="620a4-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="620a4-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="620a4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="620a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="620a4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="620a4-113">Not supported.</span></span>    |
|<span data-ttu-id="620a4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="620a4-114">Application</span></span> | <span data-ttu-id="620a4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="620a4-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="620a4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="620a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="620a4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="620a4-117">Request headers</span></span>

| <span data-ttu-id="620a4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="620a4-118">Name</span></span> | <span data-ttu-id="620a4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="620a4-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="620a4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="620a4-120">Authorization</span></span> | <span data-ttu-id="620a4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="620a4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="620a4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="620a4-123">Content-Type</span></span>  | <span data-ttu-id="620a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="620a4-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="620a4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="620a4-125">Request body</span></span>
<span data-ttu-id="620a4-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="620a4-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="620a4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="620a4-127">Response</span></span>

<span data-ttu-id="620a4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="620a4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="620a4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="620a4-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="620a4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="620a4-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="620a4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="620a4-132">Response</span></span>

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