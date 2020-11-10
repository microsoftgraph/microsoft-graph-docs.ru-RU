---
title: Создание Итемемаил
description: Создание нового Итемемаил.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da1d19a99182e7b242e162ae67b933db74cd995
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969681"
---
# <a name="create-itememail"></a><span data-ttu-id="4ad08-103">Создание Итемемаил</span><span class="sxs-lookup"><span data-stu-id="4ad08-103">Create itemEmail</span></span>

<span data-ttu-id="4ad08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ad08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ad08-105">Создание нового объекта [итемемаил](../resources/itememail.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ad08-105">Create a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ad08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ad08-106">Permissions</span></span>

<span data-ttu-id="4ad08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ad08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ad08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ad08-109">Permission type</span></span>                        | <span data-ttu-id="4ad08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ad08-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4ad08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ad08-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ad08-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ad08-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4ad08-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ad08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ad08-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ad08-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4ad08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ad08-115">Application</span></span>                            | <span data-ttu-id="4ad08-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ad08-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4ad08-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ad08-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/emails
POST /users/{id | userPrincipalName}/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="4ad08-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ad08-118">Request headers</span></span>
|<span data-ttu-id="4ad08-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4ad08-119">Name</span></span>|<span data-ttu-id="4ad08-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ad08-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ad08-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ad08-121">Authorization</span></span>|<span data-ttu-id="4ad08-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ad08-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4ad08-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ad08-124">Content-Type</span></span>|<span data-ttu-id="4ad08-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ad08-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ad08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ad08-127">Request body</span></span>
<span data-ttu-id="4ad08-128">В тексте запроса добавьте представление объекта [итемемаил](../resources/itememail.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ad08-128">In the request body, supply a JSON representation of the [itemEmail](../resources/itememail.md) object.</span></span>

<span data-ttu-id="4ad08-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [итемемаил](../resources/itememail.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ad08-129">The following table shows the properties that are possible to set when creating a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="4ad08-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ad08-130">Property</span></span>|<span data-ttu-id="4ad08-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4ad08-131">Type</span></span>|<span data-ttu-id="4ad08-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4ad08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ad08-133">address</span><span class="sxs-lookup"><span data-stu-id="4ad08-133">address</span></span>|<span data-ttu-id="4ad08-134">String</span><span class="sxs-lookup"><span data-stu-id="4ad08-134">String</span></span>|<span data-ttu-id="4ad08-135">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4ad08-135">The email address itself.</span></span>|
|<span data-ttu-id="4ad08-136">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="4ad08-136">allowedAudiences</span></span>|<span data-ttu-id="4ad08-137">String</span><span class="sxs-lookup"><span data-stu-id="4ad08-137">String</span></span>|<span data-ttu-id="4ad08-138">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="4ad08-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4ad08-139">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4ad08-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4ad08-140">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4ad08-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4ad08-141">displayName</span><span class="sxs-lookup"><span data-stu-id="4ad08-141">displayName</span></span>|<span data-ttu-id="4ad08-142">String</span><span class="sxs-lookup"><span data-stu-id="4ad08-142">String</span></span>|<span data-ttu-id="4ad08-143">Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4ad08-143">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="4ad08-144">выводов</span><span class="sxs-lookup"><span data-stu-id="4ad08-144">inference</span></span>|[<span data-ttu-id="4ad08-145">инференцедата</span><span class="sxs-lookup"><span data-stu-id="4ad08-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4ad08-146">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="4ad08-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4ad08-147">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4ad08-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4ad08-148">source</span><span class="sxs-lookup"><span data-stu-id="4ad08-148">source</span></span>|[<span data-ttu-id="4ad08-149">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="4ad08-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="4ad08-150">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="4ad08-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="4ad08-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4ad08-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4ad08-152">type</span><span class="sxs-lookup"><span data-stu-id="4ad08-152">type</span></span>|<span data-ttu-id="4ad08-153">емаилтипе</span><span class="sxs-lookup"><span data-stu-id="4ad08-153">emailType</span></span>|<span data-ttu-id="4ad08-154">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4ad08-154">The type of email address.</span></span> <span data-ttu-id="4ad08-155">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="4ad08-155">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|



## <a name="response"></a><span data-ttu-id="4ad08-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad08-156">Response</span></span>

<span data-ttu-id="4ad08-157">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [итемемаил](../resources/itememail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ad08-157">If successful, this method returns a `201 Created` response code and an [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ad08-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="4ad08-158">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="4ad08-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ad08-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/emails
Content-Type: application/json
Content-length: 383

{
  "address": "Innocenty.Popov@adventureworks.com",
}
```
# <a name="c"></a>[<span data-ttu-id="4ad08-160">C#</span><span class="sxs-lookup"><span data-stu-id="4ad08-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itememail-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ad08-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ad08-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itememail-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ad08-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ad08-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itememail-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ad08-163">Java</span><span class="sxs-lookup"><span data-stu-id="4ad08-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itememail-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4ad08-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ad08-164">Response</span></span>
<span data-ttu-id="4ad08-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4ad08-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
}
-->
``` http
HTTP/1.1 201 Created
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
  "displayName": null,
  "type": null
}
```


