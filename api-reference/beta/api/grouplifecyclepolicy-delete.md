---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 24d80596194dd83b78f3eca73531b48e0181fbf3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328517"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="f0daa-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f0daa-103">Delete groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0daa-104">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0daa-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0daa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0daa-105">Permissions</span></span>

<span data-ttu-id="f0daa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0daa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0daa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0daa-108">Permission type</span></span>      | <span data-ttu-id="f0daa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0daa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0daa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0daa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0daa-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0daa-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0daa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0daa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0daa-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f0daa-113">Not supported</span></span> |
|<span data-ttu-id="f0daa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0daa-114">Application</span></span> | <span data-ttu-id="f0daa-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0daa-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0daa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0daa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="f0daa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0daa-117">Request headers</span></span>

| <span data-ttu-id="f0daa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f0daa-118">Name</span></span> | <span data-ttu-id="f0daa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f0daa-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f0daa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0daa-120">Authorization</span></span> | <span data-ttu-id="f0daa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0daa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0daa-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0daa-123">Content-Type</span></span>  | <span data-ttu-id="f0daa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0daa-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0daa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0daa-125">Request body</span></span>
<span data-ttu-id="f0daa-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0daa-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f0daa-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0daa-127">Response</span></span>

<span data-ttu-id="f0daa-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f0daa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0daa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f0daa-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f0daa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0daa-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="f0daa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0daa-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
