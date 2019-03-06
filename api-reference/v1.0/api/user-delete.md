---
title: Удаление пользователя — API Microsoft Graph
description: Описан метод удаления ресурса (объекта) user из API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba27c81e5cb6b8bc8738c419b467e686932bc7c8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258067"
---
# <a name="delete-a-user"></a><span data-ttu-id="9d3a9-103">Удалить пользователя</span><span class="sxs-lookup"><span data-stu-id="9d3a9-103">Delete a user</span></span>

<span data-ttu-id="9d3a9-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-104">Delete user.</span></span>  

<span data-ttu-id="9d3a9-105">При удалении ресурсы user перемещаются во временный контейнер, и их можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="9d3a9-106">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="9d3a9-107">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="9d3a9-107">To learn more, see [Paging](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d3a9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3a9-108">Permissions</span></span>

<span data-ttu-id="9d3a9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d3a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d3a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3a9-111">Permission type</span></span>      | <span data-ttu-id="9d3a9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d3a9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d3a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d3a9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9d3a9-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d3a9-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d3a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d3a9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d3a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-116">Not supported.</span></span>    |
|<span data-ttu-id="9d3a9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d3a9-117">Application</span></span> | <span data-ttu-id="9d3a9-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3a9-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d3a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d3a9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="9d3a9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d3a9-120">Request headers</span></span>

| <span data-ttu-id="9d3a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d3a9-121">Header</span></span>       | <span data-ttu-id="9d3a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d3a9-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9d3a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d3a9-123">Authorization</span></span>  | <span data-ttu-id="9d3a9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9d3a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d3a9-126">Request body</span></span>

<span data-ttu-id="9d3a9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d3a9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3a9-128">Response</span></span>

<span data-ttu-id="9d3a9-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d3a9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9d3a9-131">Example</span></span>

## <a name="request"></a><span data-ttu-id="9d3a9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d3a9-132">Request</span></span>

<span data-ttu-id="9d3a9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
### <a name="response"></a><span data-ttu-id="9d3a9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3a9-134">Response</span></span>

<span data-ttu-id="9d3a9-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d3a9-135">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
