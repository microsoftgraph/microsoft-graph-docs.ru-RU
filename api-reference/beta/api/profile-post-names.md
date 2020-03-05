---
title: Создание personName
description: Используйте этот API, чтобы создать новый personName в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: dd9b66db16f3c9146b47e917d9417ac7bb7e7adb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455094"
---
# <a name="create-personname"></a><span data-ttu-id="06604-103">Создание personName</span><span class="sxs-lookup"><span data-stu-id="06604-103">Create personName</span></span>

<span data-ttu-id="06604-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06604-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06604-105">Используйте этот API, чтобы создать новый объект [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="06604-105">Use this API to create a new [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06604-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06604-106">Permissions</span></span>

<span data-ttu-id="06604-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06604-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06604-109">Permission type</span></span>                        | <span data-ttu-id="06604-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06604-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="06604-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06604-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06604-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="06604-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="06604-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06604-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06604-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="06604-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="06604-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06604-115">Application</span></span>                            | <span data-ttu-id="06604-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="06604-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06604-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06604-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/names
```

## <a name="request-headers"></a><span data-ttu-id="06604-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06604-118">Request headers</span></span>

| <span data-ttu-id="06604-119">Имя</span><span class="sxs-lookup"><span data-stu-id="06604-119">Name</span></span>           |<span data-ttu-id="06604-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06604-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="06604-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06604-121">Authorization</span></span>  | <span data-ttu-id="06604-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06604-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="06604-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06604-124">Content-Type</span></span>   | <span data-ttu-id="06604-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06604-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06604-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="06604-127">Request body</span></span>

<span data-ttu-id="06604-128">В тексте запроса добавьте представление объекта [PersonName](../resources/personname.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06604-128">In the request body, supply a JSON representation of [personName](../resources/personname.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="06604-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="06604-129">Response</span></span>

<span data-ttu-id="06604-130">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06604-130">If successful, this method returns `201, Created` response code and a new [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06604-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="06604-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06604-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06604-132">Request</span></span>

<span data-ttu-id="06604-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06604-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06604-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="06604-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personname_from_profilev2"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/names
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```
# <a name="c"></a>[<span data-ttu-id="06604-135">C#</span><span class="sxs-lookup"><span data-stu-id="06604-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personname-from-profilev2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06604-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06604-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personname-from-profilev2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06604-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06604-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personname-from-profilev2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06604-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="06604-138">Response</span></span>

<span data-ttu-id="06604-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06604-139">The following is an example of the response.</span></span>

> <span data-ttu-id="06604-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06604-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "first": "first-value",
  "initials": "initials-value",
  "last": "last-value",
  "languageTag": "languageTag-value",
  "maiden": "maiden-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create personName",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
