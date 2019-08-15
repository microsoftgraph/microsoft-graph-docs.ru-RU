---
title: 'Тииндикатор: Делететииндикаторс'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 80976240be10ee6a28ec75712f175fe0d20bd153
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409319"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="9e940-103">Тииндикатор: Делететииндикаторс</span><span class="sxs-lookup"><span data-stu-id="9e940-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e940-104">Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.</span><span class="sxs-lookup"><span data-stu-id="9e940-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e940-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e940-105">Permissions</span></span>

<span data-ttu-id="9e940-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e940-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e940-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e940-108">Permission type</span></span> | <span data-ttu-id="9e940-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e940-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e940-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e940-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e940-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9e940-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="9e940-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e940-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e940-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e940-113">Not supported.</span></span> |
| <span data-ttu-id="9e940-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e940-114">Application</span></span>                            | <span data-ttu-id="9e940-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9e940-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e940-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e940-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="9e940-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e940-117">Request headers</span></span>

| <span data-ttu-id="9e940-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9e940-118">Name</span></span>          | <span data-ttu-id="9e940-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9e940-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9e940-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e940-120">Authorization</span></span> | <span data-ttu-id="9e940-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9e940-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e940-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e940-122">Request body</span></span>

<span data-ttu-id="9e940-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9e940-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9e940-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="9e940-124">Parameter</span></span>    | <span data-ttu-id="9e940-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9e940-125">Type</span></span>        | <span data-ttu-id="9e940-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9e940-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e940-127">значение</span><span class="sxs-lookup"><span data-stu-id="9e940-127">value</span></span>|<span data-ttu-id="9e940-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9e940-128">String collection</span></span>| <span data-ttu-id="9e940-129">Коллекция Тииндикатор `id`s, которую необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="9e940-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="9e940-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e940-130">Response</span></span>

<span data-ttu-id="9e940-131">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e940-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e940-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e940-132">Examples</span></span>

<span data-ttu-id="9e940-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9e940-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9e940-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e940-134">Request</span></span>

<span data-ttu-id="9e940-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e940-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9e940-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e940-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators
Content-type: application/json

{
  "value": [
    "id-value1",
    "id-value2"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9e940-137">C#</span><span class="sxs-lookup"><span data-stu-id="9e940-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e940-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e940-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9e940-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9e940-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e940-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e940-140">Response</span></span>

<span data-ttu-id="9e940-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9e940-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9e940-142">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9e940-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9e940-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e940-143">All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
