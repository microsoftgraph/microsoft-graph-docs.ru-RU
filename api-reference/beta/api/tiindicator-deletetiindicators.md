---
title: 'Тииндикатор: Делететииндикаторс'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 98059d636e58ad0fc4f9bccc2587b50a72e5b3d3
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637579"
---
# <a name="tiindicator-deletetiindicators"></a><span data-ttu-id="a9a86-103">Тииндикатор: Делететииндикаторс</span><span class="sxs-lookup"><span data-stu-id="a9a86-103">tiIndicator: deleteTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9a86-104">Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов.</span><span class="sxs-lookup"><span data-stu-id="a9a86-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9a86-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9a86-105">Permissions</span></span>

<span data-ttu-id="a9a86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9a86-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9a86-108">Permission type</span></span> | <span data-ttu-id="a9a86-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9a86-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9a86-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9a86-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9a86-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a9a86-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="a9a86-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9a86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9a86-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9a86-113">Not supported.</span></span> |
| <span data-ttu-id="a9a86-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9a86-114">Application</span></span>                            | <span data-ttu-id="a9a86-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a9a86-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9a86-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9a86-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="a9a86-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9a86-117">Request headers</span></span>

| <span data-ttu-id="a9a86-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a9a86-118">Name</span></span>          | <span data-ttu-id="a9a86-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a9a86-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a9a86-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9a86-120">Authorization</span></span> | <span data-ttu-id="a9a86-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a9a86-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9a86-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9a86-122">Request body</span></span>

<span data-ttu-id="a9a86-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a9a86-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a9a86-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="a9a86-124">Parameter</span></span>    | <span data-ttu-id="a9a86-125">Тип</span><span class="sxs-lookup"><span data-stu-id="a9a86-125">Type</span></span>        | <span data-ttu-id="a9a86-126">Описание</span><span class="sxs-lookup"><span data-stu-id="a9a86-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9a86-127">значение</span><span class="sxs-lookup"><span data-stu-id="a9a86-127">value</span></span>|<span data-ttu-id="a9a86-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9a86-128">String collection</span></span>| <span data-ttu-id="a9a86-129">Коллекция Тииндикатор `id`s, которую необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="a9a86-129">Collection of tiIndicator `id`s to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="a9a86-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9a86-130">Response</span></span>

<span data-ttu-id="a9a86-131">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9a86-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9a86-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="a9a86-132">Examples</span></span>

<span data-ttu-id="a9a86-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a9a86-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a9a86-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9a86-134">Request</span></span>

<span data-ttu-id="a9a86-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9a86-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9a86-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9a86-136">Response</span></span>

<span data-ttu-id="a9a86-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a9a86-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a9a86-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a9a86-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a9a86-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9a86-139">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a9a86-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="a9a86-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a9a86-141">Языках</span><span class="sxs-lookup"><span data-stu-id="a9a86-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9a86-142">Язык</span><span class="sxs-lookup"><span data-stu-id="a9a86-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicators-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-deletetiindicators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
