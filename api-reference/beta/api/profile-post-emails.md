---
title: Создание объекта itemEmail
description: Создание объекта itemEmail.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 3577a0daa807c7f5016ae34b22174ffd1c2fe813
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819542"
---
# <a name="create-itememail"></a><span data-ttu-id="cf177-103">Создание объекта itemEmail</span><span class="sxs-lookup"><span data-stu-id="cf177-103">Create itemEmail</span></span>

<span data-ttu-id="cf177-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf177-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf177-105">Создание объекта [itemEmail](../resources/itememail.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="cf177-105">Create a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf177-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf177-106">Permissions</span></span>

<span data-ttu-id="cf177-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf177-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf177-109">Permission type</span></span>                        | <span data-ttu-id="cf177-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf177-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf177-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf177-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf177-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf177-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cf177-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf177-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf177-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf177-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cf177-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf177-115">Application</span></span>                            | <span data-ttu-id="cf177-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf177-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="cf177-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf177-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/emails
POST /users/{id | userPrincipalName}/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="cf177-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf177-118">Request headers</span></span>
|<span data-ttu-id="cf177-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cf177-119">Name</span></span>|<span data-ttu-id="cf177-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cf177-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cf177-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf177-121">Authorization</span></span>|<span data-ttu-id="cf177-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf177-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cf177-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf177-124">Content-Type</span></span>|<span data-ttu-id="cf177-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf177-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf177-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf177-127">Request body</span></span>
<span data-ttu-id="cf177-128">Представьте в тексте запроса описание объекта [itemEmail в формате JSON.](../resources/itememail.md)</span><span class="sxs-lookup"><span data-stu-id="cf177-128">In the request body, supply a JSON representation of the [itemEmail](../resources/itememail.md) object.</span></span>

<span data-ttu-id="cf177-129">В таблице ниже приведены свойства, которые можно установить при создании нового [объекта itemEmail](../resources/itememail.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="cf177-129">The following table shows the properties that are possible to set when creating a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="cf177-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf177-130">Property</span></span>|<span data-ttu-id="cf177-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cf177-131">Type</span></span>|<span data-ttu-id="cf177-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cf177-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf177-133">address</span><span class="sxs-lookup"><span data-stu-id="cf177-133">address</span></span>|<span data-ttu-id="cf177-134">String</span><span class="sxs-lookup"><span data-stu-id="cf177-134">String</span></span>|<span data-ttu-id="cf177-135">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cf177-135">The email address itself.</span></span>|
|<span data-ttu-id="cf177-136">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="cf177-136">allowedAudiences</span></span>|<span data-ttu-id="cf177-137">String</span><span class="sxs-lookup"><span data-stu-id="cf177-137">String</span></span>|<span data-ttu-id="cf177-138">Аудитории, которые могут просматривать значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="cf177-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="cf177-139">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="cf177-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="cf177-140">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cf177-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cf177-141">displayName</span><span class="sxs-lookup"><span data-stu-id="cf177-141">displayName</span></span>|<span data-ttu-id="cf177-142">String</span><span class="sxs-lookup"><span data-stu-id="cf177-142">String</span></span>|<span data-ttu-id="cf177-143">Имя или метка, сопоставленные пользователем с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cf177-143">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="cf177-144">inference</span><span class="sxs-lookup"><span data-stu-id="cf177-144">inference</span></span>|[<span data-ttu-id="cf177-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="cf177-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="cf177-146">Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения.</span><span class="sxs-lookup"><span data-stu-id="cf177-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="cf177-147">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="cf177-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cf177-148">source</span><span class="sxs-lookup"><span data-stu-id="cf177-148">source</span></span>|[<span data-ttu-id="cf177-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="cf177-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="cf177-150">Где значения инициированы при синхронизации из другой службы.</span><span class="sxs-lookup"><span data-stu-id="cf177-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="cf177-151">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="cf177-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="cf177-152">type</span><span class="sxs-lookup"><span data-stu-id="cf177-152">type</span></span>|<span data-ttu-id="cf177-153">emailType</span><span class="sxs-lookup"><span data-stu-id="cf177-153">emailType</span></span>|<span data-ttu-id="cf177-154">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cf177-154">The type of email address.</span></span> <span data-ttu-id="cf177-155">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="cf177-155">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|



## <a name="response"></a><span data-ttu-id="cf177-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf177-156">Response</span></span>

<span data-ttu-id="cf177-157">При успешном выполнении этот метод возвращает код `201 Created` ответа [и объект itemEmail](../resources/itememail.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf177-157">If successful, this method returns a `201 Created` response code and an [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf177-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="cf177-158">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="cf177-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf177-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cf177-160">C#</span><span class="sxs-lookup"><span data-stu-id="cf177-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itememail-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf177-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf177-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itememail-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf177-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf177-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itememail-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cf177-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf177-163">Response</span></span>
<span data-ttu-id="cf177-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf177-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
