---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 945b501b731826fab2b9072da8d662db8491289c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325989"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="cd0a3-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="cd0a3-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd0a3-104">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd0a3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd0a3-105">Permissions</span></span>

<span data-ttu-id="cd0a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd0a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cd0a3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd0a3-108">Permission type</span></span>      | <span data-ttu-id="cd0a3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd0a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd0a3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd0a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd0a3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd0a3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd0a3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd0a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd0a3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-113">Not supported.</span></span>    |
|<span data-ttu-id="cd0a3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd0a3-114">Application</span></span> | <span data-ttu-id="cd0a3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd0a3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd0a3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cd0a3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd0a3-117">Request headers</span></span>

| <span data-ttu-id="cd0a3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cd0a3-118">Name</span></span>       | <span data-ttu-id="cd0a3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cd0a3-119">Type</span></span> | <span data-ttu-id="cd0a3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cd0a3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cd0a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd0a3-121">Authorization</span></span>  | <span data-ttu-id="cd0a3-122">string</span><span class="sxs-lookup"><span data-stu-id="cd0a3-122">string</span></span>  | <span data-ttu-id="cd0a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd0a3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd0a3-125">Request body</span></span>

<span data-ttu-id="cd0a3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd0a3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd0a3-127">Response</span></span>

<span data-ttu-id="cd0a3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd0a3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cd0a3-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cd0a3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd0a3-131">Request</span></span>

<span data-ttu-id="cd0a3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="cd0a3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd0a3-133">Response</span></span>

<span data-ttu-id="cd0a3-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd0a3-134">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
