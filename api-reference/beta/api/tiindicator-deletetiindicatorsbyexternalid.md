---
title: 'Тииндикатор: Делететииндикаторсбекстерналид'
description: Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе, а не несколько запросов, а запрос содержит внешние идентификаторы, а не идентификаторы.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 41c964f02e12d420c73e005fd0d669aecbd92d0f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335252"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="9f526-103">Тииндикатор: Делететииндикаторсбекстерналид</span><span class="sxs-lookup"><span data-stu-id="9f526-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f526-104">Удалите несколько индикаторов системы анализа угроз (TI) в одном запросе вместо нескольких запросов, если запрос содержит внешние идентификаторы, а не идентификаторы.</span><span class="sxs-lookup"><span data-stu-id="9f526-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f526-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f526-105">Permissions</span></span>

<span data-ttu-id="9f526-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f526-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f526-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f526-108">Permission type</span></span>  | <span data-ttu-id="9f526-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f526-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f526-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f526-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f526-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9f526-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="9f526-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f526-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f526-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f526-113">Not supported.</span></span> |
| <span data-ttu-id="9f526-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f526-114">Application</span></span>                            | <span data-ttu-id="9f526-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9f526-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f526-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f526-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="9f526-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f526-117">Request headers</span></span>

| <span data-ttu-id="9f526-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9f526-118">Name</span></span>          | <span data-ttu-id="9f526-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9f526-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9f526-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f526-120">Authorization</span></span> | <span data-ttu-id="9f526-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9f526-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f526-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f526-122">Request body</span></span>

<span data-ttu-id="9f526-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9f526-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9f526-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="9f526-124">Parameter</span></span>    | <span data-ttu-id="9f526-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9f526-125">Type</span></span>        | <span data-ttu-id="9f526-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9f526-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9f526-127">значение</span><span class="sxs-lookup"><span data-stu-id="9f526-127">value</span></span>|<span data-ttu-id="9f526-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f526-128">String collection</span></span>| <span data-ttu-id="9f526-129">`externalIds` Коллекция объектов **тииндикатор** , которые необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="9f526-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="9f526-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f526-130">Response</span></span>

<span data-ttu-id="9f526-131">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [ресултинфо](../resources/resultinfo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f526-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f526-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f526-132">Examples</span></span>

<span data-ttu-id="9f526-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9f526-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9f526-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f526-134">Request</span></span>

<span data-ttu-id="9f526-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f526-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f526-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f526-136">Response</span></span>

<span data-ttu-id="9f526-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f526-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9f526-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f526-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f526-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f526-139">All the properties will be returned from an actual call.</span></span>

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
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
