---
title: Создание personAnniversary
description: Используйте этот API для создания нового personAnniversary.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c28e988290c239c8a7977df8eab6d3ae3a945372
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036970"
---
# <a name="create-personanniversary"></a><span data-ttu-id="8417d-103">Создание personAnniversary</span><span class="sxs-lookup"><span data-stu-id="8417d-103">Create personAnniversary</span></span>

<span data-ttu-id="8417d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8417d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8417d-105">Используйте этот API для создания нового [объекта personAnniversary](../resources/personanniversary.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="8417d-105">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8417d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8417d-106">Permissions</span></span>

<span data-ttu-id="8417d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8417d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8417d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8417d-109">Permission type</span></span>                        | <span data-ttu-id="8417d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8417d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8417d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8417d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8417d-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8417d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8417d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8417d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8417d-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8417d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8417d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8417d-115">Application</span></span>                            | <span data-ttu-id="8417d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8417d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8417d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8417d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries
POST /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="request-headers"></a><span data-ttu-id="8417d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8417d-118">Request headers</span></span>

| <span data-ttu-id="8417d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8417d-119">Name</span></span>      |<span data-ttu-id="8417d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8417d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8417d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8417d-121">Authorization</span></span>  | <span data-ttu-id="8417d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8417d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8417d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8417d-124">Content-Type</span></span>   | <span data-ttu-id="8417d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8417d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8417d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8417d-127">Request body</span></span>

<span data-ttu-id="8417d-128">В теле запроса поставляем JSON-представление [объекта personAnniversary.](../resources/personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="8417d-128">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

<span data-ttu-id="8417d-129">В следующей таблице показаны свойства, которые можно установить в новом объекте \*\*personAnniversary\*\*\*\* в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="8417d-129">The following table shows the properties that are possible to set within a new \*\*personAnniversary\*\*\*\* object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="8417d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8417d-130">Property</span></span>|<span data-ttu-id="8417d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8417d-131">Type</span></span>|<span data-ttu-id="8417d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8417d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8417d-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8417d-133">allowedAudiences</span></span>|<span data-ttu-id="8417d-134">String</span><span class="sxs-lookup"><span data-stu-id="8417d-134">String</span></span>|<span data-ttu-id="8417d-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="8417d-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8417d-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8417d-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8417d-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8417d-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8417d-138">date</span><span class="sxs-lookup"><span data-stu-id="8417d-138">date</span></span>|<span data-ttu-id="8417d-139">Date</span><span class="sxs-lookup"><span data-stu-id="8417d-139">Date</span></span>|<span data-ttu-id="8417d-140">Содержит дату, связанную с юбилейным типом.</span><span class="sxs-lookup"><span data-stu-id="8417d-140">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="8417d-141">вывод</span><span class="sxs-lookup"><span data-stu-id="8417d-141">inference</span></span>|[<span data-ttu-id="8417d-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8417d-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8417d-143">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="8417d-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8417d-144">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8417d-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8417d-145">source</span><span class="sxs-lookup"><span data-stu-id="8417d-145">source</span></span>|[<span data-ttu-id="8417d-146">personDataSource</span><span class="sxs-lookup"><span data-stu-id="8417d-146">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8417d-147">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="8417d-147">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8417d-148">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="8417d-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8417d-149">type</span><span class="sxs-lookup"><span data-stu-id="8417d-149">type</span></span>|<span data-ttu-id="8417d-150">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="8417d-150">anniversaryType</span></span>|<span data-ttu-id="8417d-151">Тип юбилея, который представляет дата.</span><span class="sxs-lookup"><span data-stu-id="8417d-151">The type of anniversary the date represents.</span></span> <span data-ttu-id="8417d-152">Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8417d-152">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="8417d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8417d-153">Response</span></span>

<span data-ttu-id="8417d-154">В случае успешной работы этот метод возвращает код отклика и новый `201, Created` [объект personAnniversary](../resources/personanniversary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8417d-154">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8417d-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="8417d-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8417d-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8417d-156">Request</span></span>

<span data-ttu-id="8417d-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8417d-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8417d-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="8417d-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "birthday",
  "date": "1980-01-08"
}
```
# <a name="c"></a>[<span data-ttu-id="8417d-159">C#</span><span class="sxs-lookup"><span data-stu-id="8417d-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personanniversary-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8417d-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8417d-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personanniversary-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8417d-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8417d-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personanniversary-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8417d-162">Java</span><span class="sxs-lookup"><span data-stu-id="8417d-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personanniversary-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8417d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8417d-163">Response</span></span>

<span data-ttu-id="8417d-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8417d-164">The following is an example of the response.</span></span>

> <span data-ttu-id="8417d-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8417d-165">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 201 Created
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
  "type": "birthday",
  "date": "Date"
}
```


