---
title: Обновление itememail
description: Обновление свойств объекта itemEmail в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e37adabbb0fc9ce8e355d2ab6e8d6a302fe14918
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577508"
---
# <a name="update-itememail"></a><span data-ttu-id="57e48-103">Обновление itememail</span><span class="sxs-lookup"><span data-stu-id="57e48-103">Update itememail</span></span>

<span data-ttu-id="57e48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57e48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57e48-105">Обновление свойств объекта [itemEmail](../resources/itememail.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="57e48-105">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="57e48-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57e48-106">Permissions</span></span>

<span data-ttu-id="57e48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57e48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57e48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57e48-109">Permission type</span></span>                        | <span data-ttu-id="57e48-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57e48-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57e48-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57e48-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57e48-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e48-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="57e48-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57e48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57e48-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e48-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="57e48-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57e48-115">Application</span></span>                            | <span data-ttu-id="57e48-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e48-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="57e48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57e48-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/emails/{id}
PATCH /users/{id | userPrincipalName}/profile/emails/{id}
```

## <a name="request-headers"></a><span data-ttu-id="57e48-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57e48-118">Request headers</span></span>
|<span data-ttu-id="57e48-119">Имя</span><span class="sxs-lookup"><span data-stu-id="57e48-119">Name</span></span>|<span data-ttu-id="57e48-120">Описание</span><span class="sxs-lookup"><span data-stu-id="57e48-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="57e48-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57e48-121">Authorization</span></span>|<span data-ttu-id="57e48-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57e48-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="57e48-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57e48-124">Content-Type</span></span>|<span data-ttu-id="57e48-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57e48-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57e48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57e48-127">Request body</span></span>

<span data-ttu-id="57e48-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="57e48-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="57e48-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="57e48-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="57e48-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="57e48-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="57e48-131">В следующей таблице показаны свойства, которые можно обновить в существующем объекте [itemEmail](../resources/itememail.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="57e48-131">The following table shows the properties that are possible to update within an existing [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="57e48-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="57e48-132">Property</span></span>|<span data-ttu-id="57e48-133">Тип</span><span class="sxs-lookup"><span data-stu-id="57e48-133">Type</span></span>|<span data-ttu-id="57e48-134">Описание</span><span class="sxs-lookup"><span data-stu-id="57e48-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57e48-135">address</span><span class="sxs-lookup"><span data-stu-id="57e48-135">address</span></span>|<span data-ttu-id="57e48-136">String</span><span class="sxs-lookup"><span data-stu-id="57e48-136">String</span></span>|<span data-ttu-id="57e48-137">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="57e48-137">The email address itself.</span></span>|
|<span data-ttu-id="57e48-138">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="57e48-138">allowedAudiences</span></span>|<span data-ttu-id="57e48-139">String</span><span class="sxs-lookup"><span data-stu-id="57e48-139">String</span></span>|<span data-ttu-id="57e48-140">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="57e48-140">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="57e48-141">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="57e48-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="57e48-142">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="57e48-142">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="57e48-143">displayName</span><span class="sxs-lookup"><span data-stu-id="57e48-143">displayName</span></span>|<span data-ttu-id="57e48-144">String</span><span class="sxs-lookup"><span data-stu-id="57e48-144">String</span></span>|<span data-ttu-id="57e48-145">Имя или метка, которые пользователь связал с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="57e48-145">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="57e48-146">вывод</span><span class="sxs-lookup"><span data-stu-id="57e48-146">inference</span></span>|[<span data-ttu-id="57e48-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="57e48-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="57e48-148">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="57e48-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="57e48-149">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="57e48-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="57e48-150">source</span><span class="sxs-lookup"><span data-stu-id="57e48-150">source</span></span>|[<span data-ttu-id="57e48-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="57e48-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="57e48-152">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="57e48-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="57e48-153">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="57e48-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="57e48-154">type</span><span class="sxs-lookup"><span data-stu-id="57e48-154">type</span></span>|<span data-ttu-id="57e48-155">emailType</span><span class="sxs-lookup"><span data-stu-id="57e48-155">emailType</span></span>|<span data-ttu-id="57e48-156">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="57e48-156">The type of email address.</span></span> <span data-ttu-id="57e48-157">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="57e48-157">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="57e48-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="57e48-158">Response</span></span>

<span data-ttu-id="57e48-159">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект itemEmail](../resources/itememail.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="57e48-159">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57e48-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="57e48-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57e48-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="57e48-161">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="57e48-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="57e48-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/emails/{id}
Content-Type: application/json
Content-length: 383

{
  "displayName": "Business Email",
  "type": "work"
}
```
# <a name="c"></a>[<span data-ttu-id="57e48-163">C#</span><span class="sxs-lookup"><span data-stu-id="57e48-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57e48-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57e48-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57e48-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57e48-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="57e48-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="57e48-166">Response</span></span>
<span data-ttu-id="57e48-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57e48-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
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
  "address": "Innocenty.Popov@adventureworks.com",
  "displayName": "Business Email",
  "type": "work"
}
```


