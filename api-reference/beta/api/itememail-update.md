---
title: Обновление итемемаил
description: Обновление свойств объекта Итемемаил в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6a6b067ff285ee952068ff4db4177664f3dbf1e6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808062"
---
# <a name="update-itememail"></a><span data-ttu-id="c065c-103">Обновление итемемаил</span><span class="sxs-lookup"><span data-stu-id="c065c-103">Update itememail</span></span>

<span data-ttu-id="c065c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c065c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c065c-105">Обновление свойств объекта [итемемаил](../resources/itememail.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="c065c-105">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c065c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c065c-106">Permissions</span></span>

<span data-ttu-id="c065c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c065c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c065c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c065c-109">Permission type</span></span>                        | <span data-ttu-id="c065c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c065c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c065c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c065c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c065c-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c065c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c065c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c065c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c065c-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c065c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c065c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c065c-115">Application</span></span>                            | <span data-ttu-id="c065c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c065c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="c065c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c065c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/emails/{id}
PATCH /users/{id | userPrincipalName}/profile/emails/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c065c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c065c-118">Request headers</span></span>
|<span data-ttu-id="c065c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c065c-119">Name</span></span>|<span data-ttu-id="c065c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c065c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c065c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c065c-121">Authorization</span></span>|<span data-ttu-id="c065c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c065c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c065c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c065c-124">Content-Type</span></span>|<span data-ttu-id="c065c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c065c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c065c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c065c-127">Request body</span></span>

<span data-ttu-id="c065c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c065c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c065c-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c065c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c065c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c065c-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="c065c-131">В следующей таблице приведены свойства, которые можно обновлять в существующем объекте [итемемаил](../resources/itememail.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="c065c-131">The following table shows the properties that are possible to update within an existing [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="c065c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="c065c-132">Property</span></span>|<span data-ttu-id="c065c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c065c-133">Type</span></span>|<span data-ttu-id="c065c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c065c-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c065c-135">address</span><span class="sxs-lookup"><span data-stu-id="c065c-135">address</span></span>|<span data-ttu-id="c065c-136">String</span><span class="sxs-lookup"><span data-stu-id="c065c-136">String</span></span>|<span data-ttu-id="c065c-137">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c065c-137">The email address itself.</span></span>|
|<span data-ttu-id="c065c-138">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="c065c-138">allowedAudiences</span></span>|<span data-ttu-id="c065c-139">String</span><span class="sxs-lookup"><span data-stu-id="c065c-139">String</span></span>|<span data-ttu-id="c065c-140">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="c065c-140">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="c065c-141">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="c065c-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="c065c-142">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c065c-142">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c065c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c065c-143">displayName</span></span>|<span data-ttu-id="c065c-144">String</span><span class="sxs-lookup"><span data-stu-id="c065c-144">String</span></span>|<span data-ttu-id="c065c-145">Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c065c-145">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="c065c-146">выводов</span><span class="sxs-lookup"><span data-stu-id="c065c-146">inference</span></span>|[<span data-ttu-id="c065c-147">инференцедата</span><span class="sxs-lookup"><span data-stu-id="c065c-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="c065c-148">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="c065c-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="c065c-149">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="c065c-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c065c-150">source</span><span class="sxs-lookup"><span data-stu-id="c065c-150">source</span></span>|[<span data-ttu-id="c065c-151">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="c065c-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="c065c-152">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="c065c-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="c065c-153">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="c065c-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c065c-154">type</span><span class="sxs-lookup"><span data-stu-id="c065c-154">type</span></span>|<span data-ttu-id="c065c-155">емаилтипе</span><span class="sxs-lookup"><span data-stu-id="c065c-155">emailType</span></span>|<span data-ttu-id="c065c-156">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c065c-156">The type of email address.</span></span> <span data-ttu-id="c065c-157">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="c065c-157">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="c065c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c065c-158">Response</span></span>

<span data-ttu-id="c065c-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [итемемаил](../resources/itememail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c065c-159">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c065c-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="c065c-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c065c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c065c-161">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="c065c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="c065c-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/emails/{id}
Content-Type: application/json
Content-length: 383

{
  "displayName": "Business Email",
  "type": "work"
}
```
# <a name="c"></a>[<span data-ttu-id="c065c-163">C#</span><span class="sxs-lookup"><span data-stu-id="c065c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c065c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c065c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c065c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c065c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c065c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c065c-166">Response</span></span>
<span data-ttu-id="c065c-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c065c-167">**Note:** The response object shown here might be shortened for readability.</span></span>
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
