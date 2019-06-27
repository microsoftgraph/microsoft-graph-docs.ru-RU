---
title: 'Тииндикатор: Упдатетииндикаторс'
description: Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: af371d5f2da6fdbe8dcc42199a1b50dffd8594ff
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270632"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="4b7fe-103">Тииндикатор: Упдатетииндикаторс</span><span class="sxs-lookup"><span data-stu-id="4b7fe-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b7fe-104">Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b7fe-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b7fe-105">Permissions</span></span>

<span data-ttu-id="4b7fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b7fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b7fe-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b7fe-108">Permission type</span></span>   | <span data-ttu-id="4b7fe-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b7fe-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b7fe-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b7fe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b7fe-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4b7fe-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="4b7fe-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b7fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b7fe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-113">Not supported.</span></span> |
| <span data-ttu-id="4b7fe-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b7fe-114">Application</span></span>                            | <span data-ttu-id="4b7fe-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="4b7fe-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b7fe-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b7fe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="4b7fe-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b7fe-117">Request headers</span></span>

| <span data-ttu-id="4b7fe-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4b7fe-118">Name</span></span>          | <span data-ttu-id="4b7fe-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4b7fe-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4b7fe-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b7fe-120">Authorization</span></span> | <span data-ttu-id="4b7fe-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4b7fe-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b7fe-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b7fe-122">Request body</span></span>

<span data-ttu-id="4b7fe-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="4b7fe-124">Дополнительные сведения о свойствах, которые можно обновлять, можно найти в [статье Update тииндикатор](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="4b7fe-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="4b7fe-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b7fe-125">Parameter</span></span>    | <span data-ttu-id="4b7fe-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4b7fe-126">Type</span></span>        | <span data-ttu-id="4b7fe-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4b7fe-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b7fe-128">значение</span><span class="sxs-lookup"><span data-stu-id="4b7fe-128">value</span></span>|<span data-ttu-id="4b7fe-129">Коллекция Тииндикатор</span><span class="sxs-lookup"><span data-stu-id="4b7fe-129">tiIndicator collection</span></span>| <span data-ttu-id="4b7fe-130">Коллекция **тииндикаторс** , которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="4b7fe-131">У каждой сущности должен быть **идентификатор** и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="4b7fe-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b7fe-132">Response</span></span>

<span data-ttu-id="4b7fe-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b7fe-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="4b7fe-134">Examples</span></span>

<span data-ttu-id="4b7fe-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4b7fe-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b7fe-136">Request</span></span>

<span data-ttu-id="4b7fe-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b7fe-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b7fe-138">Response</span></span>

<span data-ttu-id="4b7fe-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4b7fe-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4b7fe-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b7fe-141">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4b7fe-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4b7fe-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4b7fe-143">C#</span><span class="sxs-lookup"><span data-stu-id="4b7fe-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_updatetiindicators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b7fe-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="4b7fe-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_updatetiindicators-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4b7fe-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4b7fe-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tiindicator_updatetiindicators-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-updatetiindicators.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-updatetiindicators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-updatetiindicators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
