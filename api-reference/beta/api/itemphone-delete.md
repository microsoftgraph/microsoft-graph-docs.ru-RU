---
title: Удаление Итемфоне
description: Удаление объекта Итемфоне из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 87f7f468fbaf8de25dd1fdabd6840f85409e6822
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938010"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="0421a-103">Удаление Итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="0421a-103">Delete itemPhoneNumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0421a-104">Удаление объекта [итемфоне](../resources/itemphone.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="0421a-104">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0421a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0421a-105">Permissions</span></span>

<span data-ttu-id="0421a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0421a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0421a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0421a-108">Permission type</span></span>                        | <span data-ttu-id="0421a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0421a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0421a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0421a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0421a-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0421a-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0421a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0421a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0421a-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0421a-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0421a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0421a-114">Application</span></span>                            | <span data-ttu-id="0421a-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0421a-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0421a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0421a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0421a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0421a-117">Request headers</span></span>

| <span data-ttu-id="0421a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0421a-118">Name</span></span>           |<span data-ttu-id="0421a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0421a-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0421a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0421a-120">Authorization</span></span>  | <span data-ttu-id="0421a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0421a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0421a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0421a-123">Content-Type</span></span>   | <span data-ttu-id="0421a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0421a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0421a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0421a-126">Request body</span></span>

<span data-ttu-id="0421a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0421a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0421a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0421a-128">Response</span></span>

<span data-ttu-id="0421a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0421a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0421a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0421a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0421a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0421a-132">Request</span></span>

<span data-ttu-id="0421a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0421a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/phones/{id}
```

### <a name="response"></a><span data-ttu-id="0421a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0421a-134">Response</span></span>

<span data-ttu-id="0421a-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0421a-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->