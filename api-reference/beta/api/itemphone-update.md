---
title: Обновление итемфоне
description: Обновление свойств объекта итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 16c50b41e0c8a5993433b98bf394d22379ae04bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938080"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="5b085-103">Обновление итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="5b085-103">Update itemphonenumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b085-104">Обновление свойств объекта [итемфоне](../resources/itemphone.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b085-104">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b085-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b085-105">Permissions</span></span>

<span data-ttu-id="5b085-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b085-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b085-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b085-108">Permission type</span></span>                        | <span data-ttu-id="5b085-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b085-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5b085-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b085-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b085-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b085-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5b085-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b085-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b085-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b085-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5b085-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b085-114">Application</span></span>                            | <span data-ttu-id="5b085-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b085-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="5b085-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b085-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/phones/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="5b085-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b085-117">Request headers</span></span>

| <span data-ttu-id="5b085-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5b085-118">Name</span></span>           |<span data-ttu-id="5b085-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5b085-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="5b085-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b085-120">Authorization</span></span>  | <span data-ttu-id="5b085-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b085-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5b085-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b085-123">Content-Type</span></span>   | <span data-ttu-id="5b085-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b085-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b085-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b085-126">Request body</span></span>

<span data-ttu-id="5b085-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5b085-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5b085-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5b085-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5b085-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5b085-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5b085-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b085-130">Property</span></span>     | <span data-ttu-id="5b085-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b085-131">Type</span></span>        | <span data-ttu-id="5b085-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b085-132">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5b085-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5b085-133">displayName</span></span>   |<span data-ttu-id="5b085-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5b085-134">String</span></span>       | <span data-ttu-id="5b085-135">Содержит понятное имя для номера телефона.</span><span class="sxs-lookup"><span data-stu-id="5b085-135">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="5b085-136">число</span><span class="sxs-lookup"><span data-stu-id="5b085-136">number</span></span>        |<span data-ttu-id="5b085-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5b085-137">String</span></span>       | <span data-ttu-id="5b085-138">Содержит номер телефона.</span><span class="sxs-lookup"><span data-stu-id="5b085-138">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="5b085-139">type</span><span class="sxs-lookup"><span data-stu-id="5b085-139">type</span></span>          |<span data-ttu-id="5b085-140">string</span><span class="sxs-lookup"><span data-stu-id="5b085-140">string</span></span>       | <span data-ttu-id="5b085-141">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="5b085-141">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="5b085-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b085-142">Response</span></span>

<span data-ttu-id="5b085-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b085-143">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b085-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b085-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b085-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b085-145">Request</span></span>

<span data-ttu-id="5b085-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b085-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/phones/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

### <a name="response"></a><span data-ttu-id="5b085-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b085-147">Response</span></span>

<span data-ttu-id="5b085-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b085-148">The following is an example of the response.</span></span>

> <span data-ttu-id="5b085-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b085-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itemphone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->