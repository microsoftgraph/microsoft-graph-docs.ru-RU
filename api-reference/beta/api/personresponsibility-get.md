---
title: Получение Персонреспонсибилити
description: Чтение свойств и связей объекта Персонреспонсибилити.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c546d6784cad9a541778eec335bfd711b513b72b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46813159"
---
# <a name="get-personresponsibility"></a><span data-ttu-id="c4458-103">Получение Персонреспонсибилити</span><span class="sxs-lookup"><span data-stu-id="c4458-103">Get personResponsibility</span></span>
<span data-ttu-id="c4458-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4458-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4458-105">Чтение свойств и связей объекта [персонреспонсибилити](../resources/personresponsibility.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4458-105">Read the properties and relationships of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4458-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4458-106">Permissions</span></span>

<span data-ttu-id="c4458-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4458-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4458-109">Permission type</span></span>                        | <span data-ttu-id="c4458-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4458-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="c4458-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4458-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4458-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c4458-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c4458-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4458-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4458-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c4458-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c4458-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c4458-115">Application</span></span>                            | <span data-ttu-id="c4458-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c4458-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="c4458-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4458-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/responsibilities/{id}
GET /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4458-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4458-118">Optional query parameters</span></span>

<span data-ttu-id="c4458-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="c4458-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="c4458-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="c4458-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="c4458-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="c4458-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4458-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4458-122">Request headers</span></span>
|<span data-ttu-id="c4458-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c4458-123">Name</span></span>|<span data-ttu-id="c4458-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c4458-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4458-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4458-125">Authorization</span></span>|<span data-ttu-id="c4458-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4458-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4458-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4458-128">Request body</span></span>
<span data-ttu-id="c4458-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4458-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4458-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4458-130">Response</span></span>

<span data-ttu-id="c4458-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [персонреспонсибилити](../resources/personresponsibility.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4458-131">If successful, this method returns a `200 OK` response code and a [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4458-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4458-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4458-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4458-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="c4458-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4458-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "get_personresponsibility"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```
# <a name="c"></a>[<span data-ttu-id="c4458-135">C#</span><span class="sxs-lookup"><span data-stu-id="c4458-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4458-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4458-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4458-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4458-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c4458-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4458-138">Response</span></span>
<span data-ttu-id="c4458-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c4458-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
