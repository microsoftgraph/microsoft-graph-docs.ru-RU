---
title: Удаление Персонинтерест
description: Удаление объекта Персонинтерест из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ede00cecfd7ecff638a4f29ccbb42835ccd73c1c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937898"
---
# <a name="delete-personinterest"></a><span data-ttu-id="f2da9-103">Удаление Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="f2da9-103">Delete personInterest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2da9-104">Удаление объекта [персонинтерест](../resources/personinterest.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2da9-104">Delete a [personInterest](../resources/personinterest.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2da9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2da9-105">Permissions</span></span>

<span data-ttu-id="f2da9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2da9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2da9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2da9-108">Permission type</span></span>                        | <span data-ttu-id="f2da9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2da9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f2da9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2da9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2da9-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2da9-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f2da9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2da9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2da9-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2da9-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f2da9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2da9-114">Application</span></span>                            | <span data-ttu-id="f2da9-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2da9-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f2da9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2da9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f2da9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2da9-117">Request headers</span></span>

| <span data-ttu-id="f2da9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f2da9-118">Name</span></span>           |<span data-ttu-id="f2da9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f2da9-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f2da9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2da9-120">Authorization</span></span>  | <span data-ttu-id="f2da9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2da9-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="f2da9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2da9-123">Request body</span></span>

<span data-ttu-id="f2da9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2da9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2da9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2da9-125">Response</span></span>

<span data-ttu-id="f2da9-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f2da9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2da9-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2da9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2da9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2da9-129">Request</span></span>

<span data-ttu-id="f2da9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2da9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_personinterest"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/interests/{id}
```

### <a name="response"></a><span data-ttu-id="f2da9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2da9-131">Response</span></span>

<span data-ttu-id="f2da9-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f2da9-132">The following is an example of the response.</span></span>

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
  "description": "Delete personInterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
