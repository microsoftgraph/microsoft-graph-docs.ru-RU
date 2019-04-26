---
title: Удаление groupLifecyclePolicy
description: Удаление объекта groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9d58eca82c72008cb30095fe4fbfacf5a382111a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567440"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="1526e-103">Удаление groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="1526e-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="1526e-104">Удаление объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="1526e-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1526e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1526e-105">Permissions</span></span>

<span data-ttu-id="1526e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1526e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1526e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1526e-108">Permission type</span></span>      | <span data-ttu-id="1526e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1526e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1526e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1526e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1526e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1526e-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1526e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1526e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1526e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1526e-113">Not supported.</span></span>    |
|<span data-ttu-id="1526e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1526e-114">Application</span></span> | <span data-ttu-id="1526e-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1526e-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1526e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1526e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="1526e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1526e-117">Request headers</span></span>

| <span data-ttu-id="1526e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1526e-118">Name</span></span> | <span data-ttu-id="1526e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1526e-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1526e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1526e-120">Authorization</span></span> | <span data-ttu-id="1526e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1526e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1526e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1526e-123">Content-Type</span></span>  | <span data-ttu-id="1526e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1526e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1526e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1526e-125">Request body</span></span>
<span data-ttu-id="1526e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1526e-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1526e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1526e-127">Response</span></span>

<span data-ttu-id="1526e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1526e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1526e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1526e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1526e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1526e-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="1526e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1526e-132">Response</span></span>

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
