---
title: 'Тииндикатор: Делететииндикаторсбекстерналид'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов, а запрос содержит внешние идентификаторы, а не идентификаторы.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 835bc4bfdda1cda355b907e0cdf143d09bbc0ccb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270688"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="04435-103">Тииндикатор: Делететииндикаторсбекстерналид</span><span class="sxs-lookup"><span data-stu-id="04435-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04435-104">Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе вместо нескольких запросов, если запрос содержит внешние идентификаторы, а не идентификаторы.</span><span class="sxs-lookup"><span data-stu-id="04435-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="04435-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04435-105">Permissions</span></span>

<span data-ttu-id="04435-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04435-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04435-108">Permission type</span></span>  | <span data-ttu-id="04435-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04435-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04435-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04435-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="04435-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="04435-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="04435-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04435-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04435-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04435-113">Not supported.</span></span> |
| <span data-ttu-id="04435-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04435-114">Application</span></span>                            | <span data-ttu-id="04435-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="04435-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="04435-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04435-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="04435-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04435-117">Request headers</span></span>

| <span data-ttu-id="04435-118">Имя</span><span class="sxs-lookup"><span data-stu-id="04435-118">Name</span></span>          | <span data-ttu-id="04435-119">Описание</span><span class="sxs-lookup"><span data-stu-id="04435-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="04435-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04435-120">Authorization</span></span> | <span data-ttu-id="04435-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="04435-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="04435-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04435-122">Request body</span></span>

<span data-ttu-id="04435-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="04435-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04435-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="04435-124">Parameter</span></span>    | <span data-ttu-id="04435-125">Тип</span><span class="sxs-lookup"><span data-stu-id="04435-125">Type</span></span>        | <span data-ttu-id="04435-126">Описание</span><span class="sxs-lookup"><span data-stu-id="04435-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04435-127">значение</span><span class="sxs-lookup"><span data-stu-id="04435-127">value</span></span>|<span data-ttu-id="04435-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="04435-128">String collection</span></span>| <span data-ttu-id="04435-129">`externalIds` Коллекция объектов **тииндикатор** , которые необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="04435-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="04435-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="04435-130">Response</span></span>

<span data-ttu-id="04435-131">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04435-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04435-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="04435-132">Examples</span></span>

<span data-ttu-id="04435-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="04435-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="04435-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="04435-134">Request</span></span>

<span data-ttu-id="04435-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04435-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="04435-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="04435-136">Response</span></span>

<span data-ttu-id="04435-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="04435-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="04435-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04435-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="04435-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04435-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="04435-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="04435-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="04435-141">C#</span><span class="sxs-lookup"><span data-stu-id="04435-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04435-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="04435-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="04435-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="04435-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
