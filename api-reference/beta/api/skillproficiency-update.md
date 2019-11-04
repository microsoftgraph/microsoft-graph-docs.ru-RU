---
title: Обновление СкиллпрофиЦиенци
description: Обновление свойств объекта СкиллпрофиЦиенци в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6583336fbf6391103b15e8892207129d44524873
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937597"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="4ae2f-103">Обновление скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="4ae2f-103">Update skillproficiency</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ae2f-104">Обновление свойств объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-104">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ae2f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ae2f-105">Permissions</span></span>

<span data-ttu-id="4ae2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ae2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ae2f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ae2f-108">Permission type</span></span>                        | <span data-ttu-id="4ae2f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ae2f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4ae2f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ae2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ae2f-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ae2f-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4ae2f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ae2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ae2f-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ae2f-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4ae2f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ae2f-114">Application</span></span>                            | <span data-ttu-id="4ae2f-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae2f-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4ae2f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ae2f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4ae2f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ae2f-117">Request headers</span></span>

| <span data-ttu-id="4ae2f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4ae2f-118">Name</span></span>           |<span data-ttu-id="4ae2f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae2f-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4ae2f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ae2f-120">Authorization</span></span>  | <span data-ttu-id="4ae2f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4ae2f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ae2f-123">Content-Type</span></span>   | <span data-ttu-id="4ae2f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4ae2f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ae2f-126">Request body</span></span>

<span data-ttu-id="4ae2f-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4ae2f-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4ae2f-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4ae2f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ae2f-130">Property</span></span>     | <span data-ttu-id="4ae2f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4ae2f-131">Type</span></span>            | <span data-ttu-id="4ae2f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae2f-132">Description</span></span>                                                                                                                        |
|:-------------|:----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4ae2f-133">categories</span><span class="sxs-lookup"><span data-stu-id="4ae2f-133">categories</span></span>    |<span data-ttu-id="4ae2f-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4ae2f-134">String collection</span></span>| <span data-ttu-id="4ae2f-135">Содержит категории, связанные с навыком (например: личное, профессиональный, для увлечений)</span><span class="sxs-lookup"><span data-stu-id="4ae2f-135">Contains categories a user has associated with the skill (eg: personal, professional, hobby)</span></span>                                       |
|<span data-ttu-id="4ae2f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4ae2f-136">displayName</span></span>   |<span data-ttu-id="4ae2f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4ae2f-137">String</span></span>           | <span data-ttu-id="4ae2f-138">Содержит понятное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-138">Contains a friendly name for the skill.</span></span>                                                                                            | 
|<span data-ttu-id="4ae2f-139">навыки</span><span class="sxs-lookup"><span data-stu-id="4ae2f-139">proficiency</span></span>   |<span data-ttu-id="4ae2f-140">string</span><span class="sxs-lookup"><span data-stu-id="4ae2f-140">string</span></span>           | <span data-ttu-id="4ae2f-141">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-141">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4ae2f-142">webUrl</span><span class="sxs-lookup"><span data-stu-id="4ae2f-142">webUrl</span></span>        |<span data-ttu-id="4ae2f-143">String</span><span class="sxs-lookup"><span data-stu-id="4ae2f-143">String</span></span>           | <span data-ttu-id="4ae2f-144">Содержит ссылку на источник информации о навыке.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-144">Contains a link to an information source about the skill.</span></span>                                                                          |

## <a name="response"></a><span data-ttu-id="4ae2f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ae2f-145">Response</span></span>

<span data-ttu-id="4ae2f-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [скиллпрофиЦиенци](../resources/skillproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-146">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ae2f-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="4ae2f-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ae2f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ae2f-148">Request</span></span>

<span data-ttu-id="4ae2f-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-149">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ae2f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ae2f-150">Response</span></span>

<span data-ttu-id="4ae2f-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-151">The following is an example of the response.</span></span>

> <span data-ttu-id="4ae2f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ae2f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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