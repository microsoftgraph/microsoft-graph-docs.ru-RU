---
title: Обновление Персонвебсите
description: Обновление свойств объекта Персонвебсите в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b93d1ea6fa1449bf6491d3ed574e709ff2c883c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455867"
---
# <a name="update-personwebsite"></a><span data-ttu-id="8dea5-103">Обновление персонвебсите</span><span class="sxs-lookup"><span data-stu-id="8dea5-103">Update personwebsite</span></span>

<span data-ttu-id="8dea5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8dea5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dea5-105">Обновление свойств объекта [персонвебсите](../resources/personwebsite.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="8dea5-105">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8dea5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8dea5-106">Permissions</span></span>

<span data-ttu-id="8dea5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dea5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dea5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dea5-109">Permission type</span></span>                        | <span data-ttu-id="8dea5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dea5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8dea5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dea5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dea5-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8dea5-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8dea5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dea5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dea5-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8dea5-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8dea5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8dea5-115">Application</span></span>                            | <span data-ttu-id="8dea5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dea5-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8dea5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dea5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8dea5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dea5-118">Request headers</span></span>

| <span data-ttu-id="8dea5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8dea5-119">Name</span></span>           |<span data-ttu-id="8dea5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8dea5-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="8dea5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dea5-121">Authorization</span></span>  | <span data-ttu-id="8dea5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dea5-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8dea5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8dea5-124">Content-Type</span></span>   | <span data-ttu-id="8dea5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dea5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dea5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dea5-127">Request body</span></span>

<span data-ttu-id="8dea5-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8dea5-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8dea5-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8dea5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8dea5-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8dea5-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8dea5-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dea5-131">Property</span></span>     | <span data-ttu-id="8dea5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8dea5-132">Type</span></span>            | <span data-ttu-id="8dea5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8dea5-133">Description</span></span>                                                                         |
|:-------------|:----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="8dea5-134">categories</span><span class="sxs-lookup"><span data-stu-id="8dea5-134">categories</span></span>    |<span data-ttu-id="8dea5-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8dea5-135">String collection</span></span>| <span data-ttu-id="8dea5-136">Содержит категории, связанные с веб-сайтом пользователем (например, "персональный", "рецепты")</span><span class="sxs-lookup"><span data-stu-id="8dea5-136">Contains categories a user has associated with the website (eg: personal, recipes)</span></span>  |
|<span data-ttu-id="8dea5-137">description</span><span class="sxs-lookup"><span data-stu-id="8dea5-137">description</span></span>   |<span data-ttu-id="8dea5-138">String</span><span class="sxs-lookup"><span data-stu-id="8dea5-138">String</span></span>           | <span data-ttu-id="8dea5-139">Содержит описание веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="8dea5-139">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="8dea5-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8dea5-140">displayName</span></span>   |<span data-ttu-id="8dea5-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8dea5-141">String</span></span>           | <span data-ttu-id="8dea5-142">Содержит понятное имя для веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="8dea5-142">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="8dea5-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="8dea5-143">webUrl</span></span>        |<span data-ttu-id="8dea5-144">String</span><span class="sxs-lookup"><span data-stu-id="8dea5-144">String</span></span>           | <span data-ttu-id="8dea5-145">Содержит ссылку на сам веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="8dea5-145">Contains a link to the website itself.</span></span>                                              |

## <a name="response"></a><span data-ttu-id="8dea5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dea5-146">Response</span></span>

<span data-ttu-id="8dea5-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонвебсите](../resources/personwebsite.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8dea5-147">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dea5-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="8dea5-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8dea5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dea5-149">Request</span></span>

<span data-ttu-id="8dea5-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dea5-150">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8dea5-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dea5-151">Response</span></span>

<span data-ttu-id="8dea5-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8dea5-152">The following is an example of the response.</span></span>

> <span data-ttu-id="8dea5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dea5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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