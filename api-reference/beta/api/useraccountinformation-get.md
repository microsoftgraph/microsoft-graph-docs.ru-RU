---
title: Получение Усераккаунтинформатион
description: Получение свойств и связей объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: e39d4411e07d130b8974f6ff51a108acbb8da3cf
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809217"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="12a8c-103">Получение Усераккаунтинформатион</span><span class="sxs-lookup"><span data-stu-id="12a8c-103">Get userAccountInformation</span></span>

<span data-ttu-id="12a8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12a8c-105">Получение свойств и связей объекта [усераккаунтинформатион](../resources/useraccountinformation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="12a8c-105">Retrieve the properties and relationships of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="12a8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12a8c-106">Permissions</span></span>

<span data-ttu-id="12a8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12a8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a8c-109">Permission type</span></span>                        | <span data-ttu-id="12a8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a8c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="12a8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a8c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12a8c-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="12a8c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="12a8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a8c-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="12a8c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="12a8c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="12a8c-115">Application</span></span>                            | <span data-ttu-id="12a8c-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="12a8c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="12a8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a8c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/accounts/{id}
GET /users/{id | userPrincipalName}/profile/accounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12a8c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12a8c-118">Optional query parameters</span></span>

<span data-ttu-id="12a8c-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="12a8c-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="12a8c-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="12a8c-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="12a8c-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="12a8c-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12a8c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a8c-122">Request headers</span></span>

| <span data-ttu-id="12a8c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="12a8c-123">Name</span></span>          |<span data-ttu-id="12a8c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="12a8c-124">Description</span></span>                |
|:--------------|:--------------------------|
| <span data-ttu-id="12a8c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12a8c-125">Authorization</span></span> | <span data-ttu-id="12a8c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12a8c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12a8c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12a8c-128">Request body</span></span>

<span data-ttu-id="12a8c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12a8c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a8c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="12a8c-130">Response</span></span>

<span data-ttu-id="12a8c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [усераккаунтинформатион](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12a8c-131">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12a8c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="12a8c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12a8c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a8c-133">Request</span></span>

<span data-ttu-id="12a8c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a8c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```http
GET https://graph.microsoft.com/beta/user/profile/accounts/{id}
```

### <a name="response"></a><span data-ttu-id="12a8c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a8c-135">Response</span></span>

<span data-ttu-id="12a8c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12a8c-136">The following is an example of the response.</span></span>

> <span data-ttu-id="12a8c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12a8c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```
