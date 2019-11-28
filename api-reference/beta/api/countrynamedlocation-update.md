---
title: Обновление Каунтринамедлокатион
description: Обновление свойств объекта Каунтринамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81224b2c0e31ad4ade9caeca661624e1b0fe4383
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636745"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="8f297-103">Обновление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="8f297-103">Update countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f297-104">Обновление свойств объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="8f297-104">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f297-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f297-105">Permissions</span></span>

<span data-ttu-id="8f297-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f297-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f297-108">Permission type</span></span>                        | <span data-ttu-id="8f297-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f297-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f297-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f297-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f297-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="8f297-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="8f297-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f297-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f297-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f297-113">Not supported.</span></span> |
| <span data-ttu-id="8f297-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f297-114">Application</span></span>                            | <span data-ttu-id="8f297-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f297-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f297-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f297-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f297-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f297-117">Request headers</span></span>

| <span data-ttu-id="8f297-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8f297-118">Name</span></span>       | <span data-ttu-id="8f297-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8f297-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8f297-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f297-120">Authorization</span></span> | <span data-ttu-id="8f297-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f297-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f297-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f297-123">Content-type</span></span>  | <span data-ttu-id="8f297-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f297-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f297-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f297-126">Request body</span></span>

<span data-ttu-id="8f297-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8f297-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8f297-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8f297-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8f297-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8f297-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8f297-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f297-130">Property</span></span>     | <span data-ttu-id="8f297-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f297-131">Type</span></span>        | <span data-ttu-id="8f297-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f297-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f297-133">каунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="8f297-133">countriesAndRegions</span></span>|<span data-ttu-id="8f297-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8f297-134">String collection</span></span>|<span data-ttu-id="8f297-135">Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="8f297-135">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="8f297-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8f297-136">displayName</span></span>|<span data-ttu-id="8f297-137">String</span><span class="sxs-lookup"><span data-stu-id="8f297-137">String</span></span>|<span data-ttu-id="8f297-138">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="8f297-138">Human-readable name of the location.</span></span>|
|<span data-ttu-id="8f297-139">инклудеункновнкаунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="8f297-139">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="8f297-140">Логический</span><span class="sxs-lookup"><span data-stu-id="8f297-140">Boolean</span></span>|<span data-ttu-id="8f297-141">Значение, `true` если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.</span><span class="sxs-lookup"><span data-stu-id="8f297-141">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="8f297-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f297-142">Response</span></span>

<span data-ttu-id="8f297-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f297-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f297-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f297-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f297-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f297-146">Request</span></span>

<span data-ttu-id="8f297-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f297-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f297-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f297-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Updated named location without unknown countries and regions",
    "countriesAndRegions": [
        "CA",
        "IN"
    ],
    "includeUnknownCountriesAndRegions": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f297-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f297-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f297-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f297-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f297-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f297-151">Response</span></span>

<span data-ttu-id="8f297-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f297-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update countrynamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
