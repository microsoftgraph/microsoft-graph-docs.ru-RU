---
title: Обновление СкиллпрофиЦиенци
description: Обновление свойств объекта СкиллпрофиЦиенци в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 53d67c4248593b81d1091d6eb3610586a732f330
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228382"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="dd31c-103">Обновление скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="dd31c-103">Update skillproficiency</span></span>

<span data-ttu-id="dd31c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd31c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd31c-105">Обновление свойств объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd31c-105">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd31c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd31c-106">Permissions</span></span>

<span data-ttu-id="dd31c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd31c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd31c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd31c-109">Permission type</span></span>                        | <span data-ttu-id="dd31c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd31c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd31c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd31c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd31c-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dd31c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="dd31c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd31c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd31c-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dd31c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="dd31c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd31c-115">Application</span></span>                            | <span data-ttu-id="dd31c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd31c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="dd31c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd31c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd31c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd31c-118">Request headers</span></span>

| <span data-ttu-id="dd31c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dd31c-119">Name</span></span>           |<span data-ttu-id="dd31c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dd31c-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="dd31c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd31c-121">Authorization</span></span>  | <span data-ttu-id="dd31c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd31c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dd31c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd31c-124">Content-Type</span></span>   | <span data-ttu-id="dd31c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd31c-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="dd31c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd31c-127">Request body</span></span>

<span data-ttu-id="dd31c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="dd31c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dd31c-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="dd31c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dd31c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dd31c-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd31c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd31c-131">Property</span></span>     | <span data-ttu-id="dd31c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="dd31c-132">Type</span></span>            | <span data-ttu-id="dd31c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="dd31c-133">Description</span></span>                                                                                                                        |
|:-------------|:----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="dd31c-134">categories</span><span class="sxs-lookup"><span data-stu-id="dd31c-134">categories</span></span>    |<span data-ttu-id="dd31c-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd31c-135">String collection</span></span>| <span data-ttu-id="dd31c-136">Содержит категории, связанные с навыком (например: личное, профессиональный, для увлечений)</span><span class="sxs-lookup"><span data-stu-id="dd31c-136">Contains categories a user has associated with the skill (eg: personal, professional, hobby)</span></span>                                       |
|<span data-ttu-id="dd31c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dd31c-137">displayName</span></span>   |<span data-ttu-id="dd31c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="dd31c-138">String</span></span>           | <span data-ttu-id="dd31c-139">Содержит понятное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="dd31c-139">Contains a friendly name for the skill.</span></span>                                                                                            |
|<span data-ttu-id="dd31c-140">навыки</span><span class="sxs-lookup"><span data-stu-id="dd31c-140">proficiency</span></span>   |<span data-ttu-id="dd31c-141">string</span><span class="sxs-lookup"><span data-stu-id="dd31c-141">string</span></span>           | <span data-ttu-id="dd31c-142">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dd31c-142">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dd31c-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="dd31c-143">webUrl</span></span>        |<span data-ttu-id="dd31c-144">String</span><span class="sxs-lookup"><span data-stu-id="dd31c-144">String</span></span>           | <span data-ttu-id="dd31c-145">Содержит ссылку на источник информации о навыке.</span><span class="sxs-lookup"><span data-stu-id="dd31c-145">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="response"></a><span data-ttu-id="dd31c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd31c-146">Response</span></span>

<span data-ttu-id="dd31c-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [скиллпрофиЦиенци](../resources/skillproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd31c-147">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd31c-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd31c-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd31c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd31c-149">Request</span></span>

<span data-ttu-id="dd31c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd31c-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd31c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd31c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_skillproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/skills/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "displayName": "displayName-value",
  "proficiency": "proficiency-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="dd31c-152">C#</span><span class="sxs-lookup"><span data-stu-id="dd31c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd31c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd31c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd31c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd31c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd31c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd31c-155">Response</span></span>

<span data-ttu-id="dd31c-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd31c-156">The following is an example of the response.</span></span>

> <span data-ttu-id="dd31c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd31c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "displayName": "displayName-value",
  "proficiency": "proficiency-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update skillproficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
