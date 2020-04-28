---
title: 'Тииндикатор: Упдатетииндикаторс'
description: Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d4c05efc931daba5953f49f2789b54dbb163fa08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452353"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="0c4a7-103">Тииндикатор: Упдатетииндикаторс</span><span class="sxs-lookup"><span data-stu-id="0c4a7-103">tiIndicator: updateTiIndicators</span></span>

<span data-ttu-id="0c4a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c4a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c4a7-105">Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-105">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c4a7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4a7-106">Permissions</span></span>

<span data-ttu-id="0c4a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c4a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4a7-109">Permission type</span></span>   | <span data-ttu-id="0c4a7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4a7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0c4a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4a7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c4a7-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0c4a7-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="0c4a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-114">Not supported.</span></span> |
| <span data-ttu-id="0c4a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4a7-115">Application</span></span>                            | <span data-ttu-id="0c4a7-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0c4a7-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c4a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="0c4a7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c4a7-118">Request headers</span></span>

| <span data-ttu-id="0c4a7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0c4a7-119">Name</span></span>          | <span data-ttu-id="0c4a7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4a7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0c4a7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c4a7-121">Authorization</span></span> | <span data-ttu-id="0c4a7-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0c4a7-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c4a7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c4a7-123">Request body</span></span>

<span data-ttu-id="0c4a7-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="0c4a7-125">Дополнительные сведения о свойствах, которые можно обновлять, можно найти в [статье Update тииндикатор](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="0c4a7-125">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span> <span data-ttu-id="0c4a7-126">Обязательные поля для каждого Тииндикатор: `id`, `expirationDateTime`, `targetProduct`.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-126">Required fields for each tiIndicator are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="0c4a7-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c4a7-127">Parameter</span></span>    | <span data-ttu-id="0c4a7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="0c4a7-128">Type</span></span>        | <span data-ttu-id="0c4a7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4a7-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c4a7-130">значение</span><span class="sxs-lookup"><span data-stu-id="0c4a7-130">value</span></span>|<span data-ttu-id="0c4a7-131">Коллекция Тииндикатор</span><span class="sxs-lookup"><span data-stu-id="0c4a7-131">tiIndicator collection</span></span>| <span data-ttu-id="0c4a7-132">Коллекция **тииндикаторс** , которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-132">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="0c4a7-133">У каждой сущности должен быть **идентификатор** и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-133">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="0c4a7-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c4a7-134">Response</span></span>

<span data-ttu-id="0c4a7-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-135">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="0c4a7-136">При возникновении ошибки этот метод возвращает код `206 Partial Content` отклика.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-136">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="0c4a7-137">Дополнительные сведения см. в разделе [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) .</span><span class="sxs-lookup"><span data-stu-id="0c4a7-137">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="0c4a7-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="0c4a7-138">Examples</span></span>

<span data-ttu-id="0c4a7-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0c4a7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c4a7-140">Request</span></span>

<span data-ttu-id="0c4a7-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c4a7-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c4a7-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0c4a7-143">C#</span><span class="sxs-lookup"><span data-stu-id="0c4a7-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c4a7-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c4a7-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c4a7-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c4a7-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c4a7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4a7-146">Response</span></span>

<span data-ttu-id="0c4a7-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-147">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="0c4a7-148">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-148">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0c4a7-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c4a7-149">All the properties will be returned from an actual call.</span></span>

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
