---
title: Обновление Каунтринамедлокатион
description: Обновление свойств объекта Каунтринамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d68138088ed39d8c4fe4dfbcec7abcb77aa11dd3
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653743"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="b4cba-103">Обновление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="b4cba-103">Update countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4cba-104">Обновление свойств объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="b4cba-104">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4cba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4cba-105">Permissions</span></span>

<span data-ttu-id="b4cba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4cba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4cba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4cba-108">Permission type</span></span>                        | <span data-ttu-id="b4cba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4cba-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4cba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4cba-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4cba-111">Policy. ReadWrite. Кондитионалакцесс и Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="b4cba-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b4cba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4cba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4cba-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4cba-113">Not supported.</span></span> |
| <span data-ttu-id="b4cba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4cba-114">Application</span></span>                            | <span data-ttu-id="b4cba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4cba-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="b4cba-116">Этот API требует нескольких разрешений.</span><span class="sxs-lookup"><span data-stu-id="b4cba-116">This API requires multiple permissions.</span></span> <span data-ttu-id="b4cba-117">Подробнее: [Известные проблемы](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="b4cba-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="b4cba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4cba-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4cba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4cba-119">Request headers</span></span>

| <span data-ttu-id="b4cba-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b4cba-120">Name</span></span>       | <span data-ttu-id="b4cba-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cba-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b4cba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4cba-122">Authorization</span></span> | <span data-ttu-id="b4cba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4cba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4cba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4cba-125">Content-type</span></span>  | <span data-ttu-id="b4cba-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4cba-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4cba-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4cba-128">Request body</span></span>

<span data-ttu-id="b4cba-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b4cba-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b4cba-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b4cba-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b4cba-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b4cba-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4cba-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4cba-132">Property</span></span>     | <span data-ttu-id="b4cba-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b4cba-133">Type</span></span>        | <span data-ttu-id="b4cba-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cba-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4cba-135">каунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="b4cba-135">countriesAndRegions</span></span>|<span data-ttu-id="b4cba-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b4cba-136">String collection</span></span>|<span data-ttu-id="b4cba-137">Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="b4cba-137">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="b4cba-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b4cba-138">displayName</span></span>|<span data-ttu-id="b4cba-139">String</span><span class="sxs-lookup"><span data-stu-id="b4cba-139">String</span></span>|<span data-ttu-id="b4cba-140">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="b4cba-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="b4cba-141">инклудеункновнкаунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="b4cba-141">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="b4cba-142">Логический</span><span class="sxs-lookup"><span data-stu-id="b4cba-142">Boolean</span></span>|<span data-ttu-id="b4cba-143">Значение, `true` если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.</span><span class="sxs-lookup"><span data-stu-id="b4cba-143">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="b4cba-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4cba-144">Response</span></span>

<span data-ttu-id="b4cba-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4cba-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4cba-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4cba-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4cba-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4cba-148">Request</span></span>

<span data-ttu-id="b4cba-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4cba-149">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4cba-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4cba-150">Response</span></span>

<span data-ttu-id="b4cba-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4cba-151">The following is an example of the response.</span></span>

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
