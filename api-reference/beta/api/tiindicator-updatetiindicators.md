---
title: 'Тииндикатор: Упдатетииндикаторс'
description: Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d44ab406998cff70ad6292598d31d6e108f63d4f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451376"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="c1d3c-103">Тииндикатор: Упдатетииндикаторс</span><span class="sxs-lookup"><span data-stu-id="c1d3c-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1d3c-104">Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1d3c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1d3c-105">Permissions</span></span>

<span data-ttu-id="c1d3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1d3c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1d3c-108">Permission type</span></span>   | <span data-ttu-id="c1d3c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1d3c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1d3c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1d3c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1d3c-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c1d3c-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="c1d3c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1d3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1d3c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-113">Not supported.</span></span> |
| <span data-ttu-id="c1d3c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1d3c-114">Application</span></span>                            | <span data-ttu-id="c1d3c-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c1d3c-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1d3c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1d3c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="c1d3c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1d3c-117">Request headers</span></span>

| <span data-ttu-id="c1d3c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c1d3c-118">Name</span></span>          | <span data-ttu-id="c1d3c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c1d3c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c1d3c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1d3c-120">Authorization</span></span> | <span data-ttu-id="c1d3c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c1d3c-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1d3c-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1d3c-122">Request body</span></span>

<span data-ttu-id="c1d3c-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="c1d3c-124">Дополнительные сведения о свойствах, которые можно обновлять, можно найти в [статье Update тииндикатор](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="c1d3c-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="c1d3c-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="c1d3c-125">Parameter</span></span>    | <span data-ttu-id="c1d3c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c1d3c-126">Type</span></span>        | <span data-ttu-id="c1d3c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c1d3c-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1d3c-128">значение</span><span class="sxs-lookup"><span data-stu-id="c1d3c-128">value</span></span>|<span data-ttu-id="c1d3c-129">Коллекция Тииндикатор</span><span class="sxs-lookup"><span data-stu-id="c1d3c-129">tiIndicator collection</span></span>| <span data-ttu-id="c1d3c-130">Коллекция **тииндикаторс** , которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="c1d3c-131">У каждой сущности должен быть **идентификатор** и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="c1d3c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1d3c-132">Response</span></span>

<span data-ttu-id="c1d3c-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1d3c-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1d3c-134">Examples</span></span>

<span data-ttu-id="c1d3c-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c1d3c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1d3c-136">Request</span></span>

<span data-ttu-id="c1d3c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1d3c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1d3c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators",
  "isCollection":true
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
  ]
}

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1d3c-139">C#</span><span class="sxs-lookup"><span data-stu-id="c1d3c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1d3c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1d3c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1d3c-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1d3c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1d3c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1d3c-142">Response</span></span>

<span data-ttu-id="c1d3c-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c1d3c-144">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c1d3c-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1d3c-145">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
