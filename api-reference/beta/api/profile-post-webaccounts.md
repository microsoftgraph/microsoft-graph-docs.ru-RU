---
title: Создание учетной записи
description: Создайте новый объект учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d158b9ca7dcf456bf9b2c19b8c5621da316614f9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937653"
---
# <a name="create-webaccount"></a><span data-ttu-id="cea9c-103">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="cea9c-103">Create webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cea9c-104">Создайте новый объект [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="cea9c-104">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cea9c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cea9c-105">Permissions</span></span>

<span data-ttu-id="cea9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cea9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cea9c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cea9c-108">Permission type</span></span>                        | <span data-ttu-id="cea9c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cea9c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cea9c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cea9c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cea9c-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cea9c-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cea9c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cea9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cea9c-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cea9c-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cea9c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cea9c-114">Application</span></span>                            | <span data-ttu-id="cea9c-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cea9c-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cea9c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cea9c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="cea9c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cea9c-117">Request headers</span></span>

| <span data-ttu-id="cea9c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cea9c-118">Name</span></span>      |<span data-ttu-id="cea9c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cea9c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cea9c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cea9c-120">Authorization</span></span>  | <span data-ttu-id="cea9c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cea9c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cea9c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cea9c-123">Content-Type</span></span>   | <span data-ttu-id="cea9c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cea9c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cea9c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cea9c-126">Request body</span></span>

<span data-ttu-id="cea9c-127">В тексте запроса добавьте представление объекта [учетной записи](../resources/webaccount.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cea9c-127">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cea9c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cea9c-128">Response</span></span>

<span data-ttu-id="cea9c-129">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [учетной записи](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cea9c-129">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cea9c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cea9c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cea9c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cea9c-131">Request</span></span>

<span data-ttu-id="cea9c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cea9c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_webaccount_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/webAccounts
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

### <a name="response"></a><span data-ttu-id="cea9c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cea9c-133">Response</span></span>

<span data-ttu-id="cea9c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cea9c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="cea9c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cea9c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
