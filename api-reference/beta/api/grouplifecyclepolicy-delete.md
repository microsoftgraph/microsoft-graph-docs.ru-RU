---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: f92a8fbfd0a45abfdfbb1705f99eaa2d7335bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882581"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="f744e-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f744e-103">Delete groupLifecyclePolicy</span></span>

> <span data-ttu-id="f744e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f744e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f744e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f744e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f744e-106">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f744e-106">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f744e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f744e-107">Permissions</span></span>

<span data-ttu-id="f744e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f744e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f744e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f744e-110">Permission type</span></span>      | <span data-ttu-id="f744e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f744e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f744e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f744e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f744e-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f744e-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f744e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f744e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f744e-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f744e-115">Not supported</span></span> |
|<span data-ttu-id="f744e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f744e-116">Application</span></span> | <span data-ttu-id="f744e-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f744e-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f744e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f744e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="f744e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f744e-119">Request headers</span></span>

| <span data-ttu-id="f744e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f744e-120">Name</span></span> | <span data-ttu-id="f744e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f744e-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f744e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f744e-122">Authorization</span></span> | <span data-ttu-id="f744e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f744e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f744e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f744e-125">Content-Type</span></span>  | <span data-ttu-id="f744e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f744e-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f744e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f744e-127">Request body</span></span>
<span data-ttu-id="f744e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f744e-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f744e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f744e-129">Response</span></span>

<span data-ttu-id="f744e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f744e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f744e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f744e-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f744e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f744e-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="f744e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f744e-134">Response</span></span>

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
