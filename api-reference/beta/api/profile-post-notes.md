---
title: Создание заметок
description: Создание нового объекта Notes.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 139de864b9ddec90336e56e122da5f6bf6922952
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034394"
---
# <a name="create-personannotation"></a><span data-ttu-id="af1c5-103">Создание Персонаннотатион</span><span class="sxs-lookup"><span data-stu-id="af1c5-103">Create personAnnotation</span></span>
<span data-ttu-id="af1c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af1c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af1c5-105">Создание нового объекта [персонаннотатион](../resources/personannotation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="af1c5-105">Create a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af1c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af1c5-106">Permissions</span></span>

<span data-ttu-id="af1c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af1c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="af1c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af1c5-109">Permission type</span></span>                        | <span data-ttu-id="af1c5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af1c5-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="af1c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af1c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="af1c5-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af1c5-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="af1c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af1c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af1c5-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af1c5-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="af1c5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af1c5-115">Application</span></span>                            | <span data-ttu-id="af1c5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af1c5-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="af1c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af1c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/notes
POST /users/{id | userPrincipalName}/profile/notes
```

## <a name="request-headers"></a><span data-ttu-id="af1c5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af1c5-118">Request headers</span></span>
|<span data-ttu-id="af1c5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="af1c5-119">Name</span></span>|<span data-ttu-id="af1c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="af1c5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af1c5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af1c5-121">Authorization</span></span>|<span data-ttu-id="af1c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af1c5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="af1c5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af1c5-124">Content-Type</span></span>|<span data-ttu-id="af1c5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af1c5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af1c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af1c5-127">Request body</span></span>
<span data-ttu-id="af1c5-128">В тексте запроса добавьте представление объекта [персонаннотатион](../resources/personannotation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af1c5-128">In the request body, supply a JSON representation of the [personAnnotation](../resources/personannotation.md) object.</span></span>

<span data-ttu-id="af1c5-129">В следующей таблице приведены свойства, которые можно задать в новом объекте [персонаннотатион](../resources/personannotation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="af1c5-129">The following table shows the properties that are possible to set within a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="af1c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af1c5-130">Property</span></span>|<span data-ttu-id="af1c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af1c5-131">Type</span></span>|<span data-ttu-id="af1c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af1c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af1c5-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="af1c5-133">allowedAudiences</span></span>|<span data-ttu-id="af1c5-134">String</span><span class="sxs-lookup"><span data-stu-id="af1c5-134">String</span></span>|<span data-ttu-id="af1c5-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="af1c5-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="af1c5-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="af1c5-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="af1c5-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="af1c5-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="af1c5-138">описаны</span><span class="sxs-lookup"><span data-stu-id="af1c5-138">detail</span></span>|[<span data-ttu-id="af1c5-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="af1c5-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="af1c5-140">Содержит подробные сведения о самом заметке.</span><span class="sxs-lookup"><span data-stu-id="af1c5-140">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="af1c5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="af1c5-141">displayName</span></span>|<span data-ttu-id="af1c5-142">String</span><span class="sxs-lookup"><span data-stu-id="af1c5-142">String</span></span>|<span data-ttu-id="af1c5-143">Содержит понятное имя для заметки.</span><span class="sxs-lookup"><span data-stu-id="af1c5-143">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="af1c5-144">выводов</span><span class="sxs-lookup"><span data-stu-id="af1c5-144">inference</span></span>|[<span data-ttu-id="af1c5-145">инференцедата</span><span class="sxs-lookup"><span data-stu-id="af1c5-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="af1c5-146">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="af1c5-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="af1c5-147">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="af1c5-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="af1c5-148">source</span><span class="sxs-lookup"><span data-stu-id="af1c5-148">source</span></span>|[<span data-ttu-id="af1c5-149">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="af1c5-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="af1c5-150">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="af1c5-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="af1c5-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="af1c5-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="af1c5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="af1c5-152">Response</span></span>

<span data-ttu-id="af1c5-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [персонаннотатион](../resources/personannotation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af1c5-153">If successful, this method returns a `201 Created` response code and a [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af1c5-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="af1c5-154">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="af1c5-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="af1c5-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personannotation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/notes
Content-Type: application/json
Content-length: 413

{
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow, Russia."
  },
  "displayName": "About Me"
}
```
# <a name="c"></a>[<span data-ttu-id="af1c5-156">C#</span><span class="sxs-lookup"><span data-stu-id="af1c5-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personannotation-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af1c5-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af1c5-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personannotation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af1c5-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af1c5-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personannotation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="af1c5-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="af1c5-159">Response</span></span>
<span data-ttu-id="af1c5-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af1c5-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnnotation"
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
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow, Russia."
  },
  "displayName": "About Me"
}
```


