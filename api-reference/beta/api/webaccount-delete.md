---
title: Удаление учетной записи службы
description: Удаление объекта учетной записи из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 594d7556c123ce82ed422deb02114fa25ad6405d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938136"
---
# <a name="delete-webaccount"></a><span data-ttu-id="85e55-103">Удаление учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="85e55-103">Delete webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85e55-104">Удаление объекта [учетной записи](../resources/webaccount.md) из профиля пользователя.</span><span class="sxs-lookup"><span data-stu-id="85e55-104">Delete a [webAccount](../resources/webaccount.md) object from the user's profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="85e55-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85e55-105">Permissions</span></span>

<span data-ttu-id="85e55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85e55-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85e55-108">Permission type</span></span>                        | <span data-ttu-id="85e55-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85e55-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85e55-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85e55-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85e55-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="85e55-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="85e55-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85e55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85e55-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="85e55-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="85e55-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85e55-114">Application</span></span>                            | <span data-ttu-id="85e55-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e55-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="85e55-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85e55-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="85e55-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85e55-117">Request headers</span></span>

| <span data-ttu-id="85e55-118">Имя</span><span class="sxs-lookup"><span data-stu-id="85e55-118">Name</span></span>           |<span data-ttu-id="85e55-119">Описание</span><span class="sxs-lookup"><span data-stu-id="85e55-119">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="85e55-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85e55-120">Authorization</span></span>  | <span data-ttu-id="85e55-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85e55-p102">Bearer {token}. Required.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="85e55-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85e55-123">Request body</span></span>

<span data-ttu-id="85e55-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85e55-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85e55-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="85e55-125">Response</span></span>

<span data-ttu-id="85e55-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85e55-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85e55-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="85e55-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85e55-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="85e55-129">Request</span></span>

<span data-ttu-id="85e55-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85e55-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_webaccount"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
```

### <a name="response"></a><span data-ttu-id="85e55-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="85e55-131">Response</span></span>

<span data-ttu-id="85e55-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="85e55-132">The following is an example of the response.</span></span>

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
  "description": "Delete webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
