---
title: Обновление Персонанниверсари
description: Обновление свойств объекта персонанниверсари.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9297698416d89b8eff8b5d646d1e3025761f4f7b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937905"
---
# <a name="update-personanniversary"></a><span data-ttu-id="38a07-103">Обновление Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="38a07-103">Update personAnniversary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a07-104">Обновление свойств объекта [персонанниверсари](../resources/personanniversary.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="38a07-104">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38a07-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38a07-105">Permissions</span></span>

<span data-ttu-id="38a07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38a07-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38a07-108">Permission type</span></span>                        | <span data-ttu-id="38a07-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38a07-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38a07-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38a07-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="38a07-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="38a07-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38a07-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38a07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38a07-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="38a07-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38a07-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38a07-114">Application</span></span>                            | <span data-ttu-id="38a07-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a07-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="38a07-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38a07-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="38a07-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38a07-117">Request headers</span></span>

| <span data-ttu-id="38a07-118">Имя</span><span class="sxs-lookup"><span data-stu-id="38a07-118">Name</span></span>           |<span data-ttu-id="38a07-119">Описание</span><span class="sxs-lookup"><span data-stu-id="38a07-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="38a07-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38a07-120">Authorization</span></span>  | <span data-ttu-id="38a07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38a07-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="38a07-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38a07-123">Content-Type</span></span>   | <span data-ttu-id="38a07-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38a07-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38a07-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38a07-126">Request body</span></span>

<span data-ttu-id="38a07-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="38a07-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="38a07-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="38a07-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="38a07-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="38a07-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="38a07-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="38a07-130">Property</span></span>     | <span data-ttu-id="38a07-131">Тип</span><span class="sxs-lookup"><span data-stu-id="38a07-131">Type</span></span>        | <span data-ttu-id="38a07-132">Описание</span><span class="sxs-lookup"><span data-stu-id="38a07-132">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="38a07-133">date</span><span class="sxs-lookup"><span data-stu-id="38a07-133">date</span></span>          |<span data-ttu-id="38a07-134">Date</span><span class="sxs-lookup"><span data-stu-id="38a07-134">Date</span></span>         | <span data-ttu-id="38a07-135">Содержит дату, связанную с типом юбилея.</span><span class="sxs-lookup"><span data-stu-id="38a07-135">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="38a07-136">type</span><span class="sxs-lookup"><span data-stu-id="38a07-136">type</span></span>          |<span data-ttu-id="38a07-137">string</span><span class="sxs-lookup"><span data-stu-id="38a07-137">string</span></span>       | <span data-ttu-id="38a07-138">Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="38a07-138">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="38a07-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="38a07-139">Response</span></span>

<span data-ttu-id="38a07-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонанниверсари](../resources/personanniversary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38a07-140">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38a07-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="38a07-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38a07-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="38a07-142">Request</span></span>

<span data-ttu-id="38a07-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38a07-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

### <a name="response"></a><span data-ttu-id="38a07-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="38a07-144">Response</span></span>

<span data-ttu-id="38a07-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="38a07-145">The following is an example of the response.</span></span>

> <span data-ttu-id="38a07-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38a07-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personanniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
