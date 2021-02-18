---
title: Get personResponsibility
description: Чтение свойств и связей объекта personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 244313cd23c3a5635d75d3af7242df138ce253a5
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292709"
---
# <a name="get-personresponsibility"></a><span data-ttu-id="941c3-103">Get personResponsibility</span><span class="sxs-lookup"><span data-stu-id="941c3-103">Get personResponsibility</span></span>
<span data-ttu-id="941c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="941c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="941c3-105">Чтение свойств и связей объекта [personResponsibility](../resources/personresponsibility.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="941c3-105">Read the properties and relationships of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="941c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="941c3-106">Permissions</span></span>

<span data-ttu-id="941c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="941c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="941c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="941c3-109">Permission type</span></span>                        | <span data-ttu-id="941c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="941c3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="941c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="941c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="941c3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941c3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="941c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="941c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941c3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941c3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="941c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="941c3-115">Application</span></span>                            | <span data-ttu-id="941c3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941c3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="941c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="941c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/responsibilities/{id}
GET /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="941c3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="941c3-118">Optional query parameters</span></span>

<span data-ttu-id="941c3-119">Этот метод поддерживает параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="941c3-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="941c3-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятой.</span><span class="sxs-lookup"><span data-stu-id="941c3-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="941c3-121">Для оптимальной производительности выберите только подмножество необходимых свойств.</span><span class="sxs-lookup"><span data-stu-id="941c3-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="941c3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="941c3-122">Request headers</span></span>
|<span data-ttu-id="941c3-123">Имя</span><span class="sxs-lookup"><span data-stu-id="941c3-123">Name</span></span>|<span data-ttu-id="941c3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="941c3-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="941c3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="941c3-125">Authorization</span></span>|<span data-ttu-id="941c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="941c3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="941c3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="941c3-128">Request body</span></span>
<span data-ttu-id="941c3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="941c3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="941c3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="941c3-130">Response</span></span>

<span data-ttu-id="941c3-131">В случае успеха этот метод возвращает код отклика и объект `200 OK` [personResponsibility](../resources/personresponsibility.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="941c3-131">If successful, this method returns a `200 OK` response code and a [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="941c3-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="941c3-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="941c3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="941c3-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "get_personresponsibility"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="941c3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="941c3-134">Response</span></span>
<span data-ttu-id="941c3-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="941c3-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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


