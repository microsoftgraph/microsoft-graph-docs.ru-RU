---
title: 'Тииндикатор: Упдатетииндикаторс'
description: Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 91020b533b621c1ba77b2f839d4e6ffd8d7ee8ac
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30367143"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="58287-103">Тииндикатор: Упдатетииндикаторс</span><span class="sxs-lookup"><span data-stu-id="58287-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58287-104">Обновляйте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.</span><span class="sxs-lookup"><span data-stu-id="58287-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="58287-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58287-105">Permissions</span></span>

<span data-ttu-id="58287-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58287-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58287-108">Permission type</span></span>   | <span data-ttu-id="58287-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58287-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="58287-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58287-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="58287-111">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="58287-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="58287-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58287-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58287-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58287-113">Not supported.</span></span> |
| <span data-ttu-id="58287-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58287-114">Application</span></span>                            | <span data-ttu-id="58287-115">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="58287-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="58287-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58287-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="58287-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58287-117">Request headers</span></span>

| <span data-ttu-id="58287-118">Имя</span><span class="sxs-lookup"><span data-stu-id="58287-118">Name</span></span>          | <span data-ttu-id="58287-119">Описание</span><span class="sxs-lookup"><span data-stu-id="58287-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="58287-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58287-120">Authorization</span></span> | <span data-ttu-id="58287-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="58287-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="58287-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58287-122">Request body</span></span>

<span data-ttu-id="58287-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="58287-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="58287-124">Дополнительные сведения о свойствах, которые можно обновлять, можно найти в [статье Update тииндикатор](tiindicator-update.md).</span><span class="sxs-lookup"><span data-stu-id="58287-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="58287-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="58287-125">Parameter</span></span>    | <span data-ttu-id="58287-126">Тип</span><span class="sxs-lookup"><span data-stu-id="58287-126">Type</span></span>        | <span data-ttu-id="58287-127">Описание</span><span class="sxs-lookup"><span data-stu-id="58287-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="58287-128">value</span><span class="sxs-lookup"><span data-stu-id="58287-128">value</span></span>|<span data-ttu-id="58287-129">Коллекция Тииндикатор</span><span class="sxs-lookup"><span data-stu-id="58287-129">tiIndicator collection</span></span>| <span data-ttu-id="58287-130">Коллекция **тииндикаторс** , которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="58287-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="58287-131">У каждой сущности должен быть **идентификатор** и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="58287-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="58287-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="58287-132">Response</span></span>

<span data-ttu-id="58287-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58287-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58287-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="58287-134">Examples</span></span>

<span data-ttu-id="58287-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="58287-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="58287-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="58287-136">Request</span></span>

<span data-ttu-id="58287-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58287-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators"
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

### <a name="response"></a><span data-ttu-id="58287-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="58287-138">Response</span></span>

<span data-ttu-id="58287-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58287-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="58287-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="58287-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="58287-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58287-141">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
