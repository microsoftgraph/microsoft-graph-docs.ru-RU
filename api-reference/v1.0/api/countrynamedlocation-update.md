---
title: Обновление Каунтринамедлокатион
description: Обновление свойств объекта Каунтринамедлокатион.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91c297d9f82940e1578a088755144469690d33dc
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384763"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="c45a1-103">Обновление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="c45a1-103">Update countryNamedLocation</span></span>

<span data-ttu-id="c45a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c45a1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c45a1-105">Обновление свойств объекта [каунтринамедлокатион](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="c45a1-105">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c45a1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c45a1-106">Permissions</span></span>

<span data-ttu-id="c45a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c45a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c45a1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c45a1-109">Permission type</span></span>                        | <span data-ttu-id="c45a1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c45a1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c45a1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c45a1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c45a1-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="c45a1-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="c45a1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c45a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c45a1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c45a1-114">Not supported.</span></span> |
| <span data-ttu-id="c45a1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c45a1-115">Application</span></span>                            | <span data-ttu-id="c45a1-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="c45a1-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="c45a1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c45a1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c45a1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c45a1-118">Request headers</span></span>

| <span data-ttu-id="c45a1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c45a1-119">Name</span></span>       | <span data-ttu-id="c45a1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c45a1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c45a1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c45a1-121">Authorization</span></span> | <span data-ttu-id="c45a1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c45a1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c45a1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c45a1-124">Content-type</span></span>  | <span data-ttu-id="c45a1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c45a1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c45a1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c45a1-127">Request body</span></span>

<span data-ttu-id="c45a1-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c45a1-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c45a1-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c45a1-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c45a1-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c45a1-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c45a1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c45a1-131">Property</span></span>     | <span data-ttu-id="c45a1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c45a1-132">Type</span></span>        | <span data-ttu-id="c45a1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c45a1-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c45a1-134">каунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="c45a1-134">countriesAndRegions</span></span>|<span data-ttu-id="c45a1-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c45a1-135">String collection</span></span>|<span data-ttu-id="c45a1-136">Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="c45a1-136">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="c45a1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c45a1-137">displayName</span></span>|<span data-ttu-id="c45a1-138">String</span><span class="sxs-lookup"><span data-stu-id="c45a1-138">String</span></span>|<span data-ttu-id="c45a1-139">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="c45a1-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="c45a1-140">инклудеункновнкаунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="c45a1-140">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="c45a1-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="c45a1-141">Boolean</span></span>|<span data-ttu-id="c45a1-142">Значение, `true` Если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.</span><span class="sxs-lookup"><span data-stu-id="c45a1-142">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="c45a1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c45a1-143">Response</span></span>

<span data-ttu-id="c45a1-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c45a1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c45a1-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="c45a1-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c45a1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c45a1-147">Request</span></span>

<span data-ttu-id="c45a1-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c45a1-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
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

### <a name="response"></a><span data-ttu-id="c45a1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c45a1-149">Response</span></span>

<span data-ttu-id="c45a1-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c45a1-150">The following is an example of the response.</span></span>

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
