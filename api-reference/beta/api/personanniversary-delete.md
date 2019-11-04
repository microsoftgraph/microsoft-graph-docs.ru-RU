---
title: Удаление Персонанниверсари
description: Удаление объекта Персонанниверсари из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 3e936ee61dbdcedd2d5c190501b1db9dbc6173d5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937919"
---
# <a name="delete-personanniversary"></a><span data-ttu-id="a0607-103">Удаление Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="a0607-103">Delete personAnniversary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0607-104">Удаление объекта [персонанниверсари](../resources/personanniversary.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0607-104">Delete a [personAnniversary](../resources/personanniversary.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0607-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0607-105">Permissions</span></span>

<span data-ttu-id="a0607-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0607-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0607-108">Permission type</span></span>                        | <span data-ttu-id="a0607-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0607-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0607-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0607-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0607-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a0607-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a0607-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0607-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0607-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a0607-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a0607-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0607-114">Application</span></span>                            | <span data-ttu-id="a0607-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0607-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="a0607-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0607-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="a0607-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0607-117">Request headers</span></span>

| <span data-ttu-id="a0607-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a0607-118">Name</span></span>           |<span data-ttu-id="a0607-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a0607-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a0607-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0607-120">Authorization</span></span>  | <span data-ttu-id="a0607-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0607-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="a0607-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0607-123">Request body</span></span>

<span data-ttu-id="a0607-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0607-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0607-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0607-125">Response</span></span>

<span data-ttu-id="a0607-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a0607-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0607-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a0607-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0607-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0607-129">Request</span></span>

<span data-ttu-id="a0607-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0607-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_personanniversary"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
```

### <a name="response"></a><span data-ttu-id="a0607-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0607-131">Response</span></span>

<span data-ttu-id="a0607-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a0607-132">The following is an example of the response.</span></span>

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
  "description": "Delete personAnniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
