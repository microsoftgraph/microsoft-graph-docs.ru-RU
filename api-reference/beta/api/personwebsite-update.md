---
title: Обновление Персонвебсите
description: Обновление свойств объекта Персонвебсите в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b782981d52f2092aff2d1f99d749e879910289bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937842"
---
# <a name="update-personwebsite"></a><span data-ttu-id="bd001-103">Обновление персонвебсите</span><span class="sxs-lookup"><span data-stu-id="bd001-103">Update personwebsite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd001-104">Обновление свойств объекта [персонвебсите](../resources/personwebsite.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd001-104">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd001-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd001-105">Permissions</span></span>

<span data-ttu-id="bd001-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd001-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd001-108">Permission type</span></span>                        | <span data-ttu-id="bd001-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd001-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd001-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd001-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd001-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bd001-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bd001-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd001-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd001-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bd001-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bd001-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd001-114">Application</span></span>                            | <span data-ttu-id="bd001-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd001-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="bd001-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd001-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bd001-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd001-117">Request headers</span></span>

| <span data-ttu-id="bd001-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bd001-118">Name</span></span>           |<span data-ttu-id="bd001-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bd001-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="bd001-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd001-120">Authorization</span></span>  | <span data-ttu-id="bd001-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd001-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bd001-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd001-123">Content-Type</span></span>   | <span data-ttu-id="bd001-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd001-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd001-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd001-126">Request body</span></span>

<span data-ttu-id="bd001-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="bd001-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bd001-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="bd001-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bd001-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bd001-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bd001-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd001-130">Property</span></span>     | <span data-ttu-id="bd001-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bd001-131">Type</span></span>            | <span data-ttu-id="bd001-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bd001-132">Description</span></span>                                                                         |
|:-------------|:----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="bd001-133">categories</span><span class="sxs-lookup"><span data-stu-id="bd001-133">categories</span></span>    |<span data-ttu-id="bd001-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bd001-134">String collection</span></span>| <span data-ttu-id="bd001-135">Содержит категории, связанные с веб-сайтом пользователем (например, "персональный", "рецепты")</span><span class="sxs-lookup"><span data-stu-id="bd001-135">Contains categories a user has associated with the website (eg: personal, recipes)</span></span>  |
|<span data-ttu-id="bd001-136">description</span><span class="sxs-lookup"><span data-stu-id="bd001-136">description</span></span>   |<span data-ttu-id="bd001-137">String</span><span class="sxs-lookup"><span data-stu-id="bd001-137">String</span></span>           | <span data-ttu-id="bd001-138">Содержит описание веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="bd001-138">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="bd001-139">displayName</span><span class="sxs-lookup"><span data-stu-id="bd001-139">displayName</span></span>   |<span data-ttu-id="bd001-140">Строка</span><span class="sxs-lookup"><span data-stu-id="bd001-140">String</span></span>           | <span data-ttu-id="bd001-141">Содержит понятное имя для веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="bd001-141">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="bd001-142">webUrl</span><span class="sxs-lookup"><span data-stu-id="bd001-142">webUrl</span></span>        |<span data-ttu-id="bd001-143">String</span><span class="sxs-lookup"><span data-stu-id="bd001-143">String</span></span>           | <span data-ttu-id="bd001-144">Содержит ссылку на сам веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="bd001-144">Contains a link to the website itself.</span></span>                                              |

## <a name="response"></a><span data-ttu-id="bd001-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd001-145">Response</span></span>

<span data-ttu-id="bd001-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонвебсите](../resources/personwebsite.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd001-146">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd001-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd001-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd001-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd001-148">Request</span></span>

<span data-ttu-id="bd001-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd001-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_personwebsite"
}-->

```http
PATCH https://graph.microsoft.com/beta/user/profile/websites/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

### <a name="response"></a><span data-ttu-id="bd001-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd001-150">Response</span></span>

<span data-ttu-id="bd001-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd001-151">The following is an example of the response.</span></span>

> <span data-ttu-id="bd001-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd001-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personwebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->