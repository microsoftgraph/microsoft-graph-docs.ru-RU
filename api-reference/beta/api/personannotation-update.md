---
title: Обновление personAnnotation
description: Обновление свойств объекта personAnnotation.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a86467b01d6072f4a14dad6fc5d1a6838249899b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774168"
---
# <a name="update-personannotation"></a><span data-ttu-id="81728-103">Обновление personAnnotation</span><span class="sxs-lookup"><span data-stu-id="81728-103">Update personAnnotation</span></span>
<span data-ttu-id="81728-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81728-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81728-105">Обновление свойств объекта [personAnnotation](../resources/personannotation.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="81728-105">Update the properties of a [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81728-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81728-106">Permissions</span></span>

<span data-ttu-id="81728-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81728-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81728-109">Permission type</span></span>                        | <span data-ttu-id="81728-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81728-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="81728-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81728-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="81728-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81728-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="81728-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81728-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81728-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81728-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="81728-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81728-115">Application</span></span>                            | <span data-ttu-id="81728-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81728-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="81728-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81728-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/notes/{id}
PATCH /users/{id | userPrincipalName}/profile/notes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="81728-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81728-118">Request headers</span></span>
|<span data-ttu-id="81728-119">Имя</span><span class="sxs-lookup"><span data-stu-id="81728-119">Name</span></span>|<span data-ttu-id="81728-120">Описание</span><span class="sxs-lookup"><span data-stu-id="81728-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81728-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81728-121">Authorization</span></span>|<span data-ttu-id="81728-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81728-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="81728-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81728-124">Content-Type</span></span>|<span data-ttu-id="81728-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81728-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81728-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81728-127">Request body</span></span>

<span data-ttu-id="81728-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="81728-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="81728-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="81728-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="81728-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="81728-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="81728-131">В следующей таблице показаны свойства, которые можно обновить в существующем объекте [personAnnotation](../resources/personannotation.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="81728-131">The following table shows the properties that are possible to update within an existing [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="81728-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="81728-132">Property</span></span>|<span data-ttu-id="81728-133">Тип</span><span class="sxs-lookup"><span data-stu-id="81728-133">Type</span></span>|<span data-ttu-id="81728-134">Описание</span><span class="sxs-lookup"><span data-stu-id="81728-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81728-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="81728-135">allowedAudiences</span></span>|<span data-ttu-id="81728-136">String</span><span class="sxs-lookup"><span data-stu-id="81728-136">String</span></span>|<span data-ttu-id="81728-137">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="81728-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="81728-138">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="81728-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="81728-139">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="81728-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="81728-140">подробные</span><span class="sxs-lookup"><span data-stu-id="81728-140">detail</span></span>|[<span data-ttu-id="81728-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="81728-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="81728-142">Содержит сведения о самой заметке.</span><span class="sxs-lookup"><span data-stu-id="81728-142">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="81728-143">displayName</span><span class="sxs-lookup"><span data-stu-id="81728-143">displayName</span></span>|<span data-ttu-id="81728-144">String</span><span class="sxs-lookup"><span data-stu-id="81728-144">String</span></span>|<span data-ttu-id="81728-145">Содержит удобное имя для заметки.</span><span class="sxs-lookup"><span data-stu-id="81728-145">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="81728-146">вывод</span><span class="sxs-lookup"><span data-stu-id="81728-146">inference</span></span>|[<span data-ttu-id="81728-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="81728-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="81728-148">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="81728-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="81728-149">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="81728-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="81728-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="81728-150">Response</span></span>

<span data-ttu-id="81728-151">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [personAnnotation](../resources/personannotation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="81728-151">If successful, this method returns a `200 OK` response code and an updated [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81728-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="81728-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81728-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="81728-153">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="81728-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="81728-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personannotation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/notes/{id}
Content-Type: application/json
Content-length: 413

{
  "allowedAudiences": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="81728-155">C#</span><span class="sxs-lookup"><span data-stu-id="81728-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personannotation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81728-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81728-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personannotation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81728-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81728-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personannotation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81728-158">Java</span><span class="sxs-lookup"><span data-stu-id="81728-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personannotation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="81728-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="81728-159">Response</span></span>
<span data-ttu-id="81728-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="81728-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
    "@odata.type": "microsoft.graph.personAnnotation"
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
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow."
  },
  "displayName": "About Me"
}
```



