---
title: Получение Аппликатионтемплате
description: Получение свойств и связей объекта аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 152c09467253cd09d55acf17732b11414063616a
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147931"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="efa5a-103">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="efa5a-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efa5a-104">Получение свойств объекта [аппликатионтемплате](../resources/applicationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="efa5a-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="efa5a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efa5a-105">Permissions</span></span>

<span data-ttu-id="efa5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="efa5a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efa5a-108">Permission type</span></span>                        | <span data-ttu-id="efa5a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efa5a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="efa5a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efa5a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="efa5a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="efa5a-111">None.</span></span> |
| <span data-ttu-id="efa5a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efa5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efa5a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efa5a-113">Not supported.</span></span> |
| <span data-ttu-id="efa5a-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="efa5a-114">Application</span></span>                            | <span data-ttu-id="efa5a-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="efa5a-115">None.</span></span> |

<span data-ttu-id="efa5a-116">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="efa5a-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="efa5a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efa5a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efa5a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efa5a-118">Optional query parameters</span></span>

<span data-ttu-id="efa5a-119">С помощью параметра `$select` запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="efa5a-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="efa5a-120">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="efa5a-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="efa5a-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="efa5a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="efa5a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efa5a-122">Request headers</span></span>

| <span data-ttu-id="efa5a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="efa5a-123">Name</span></span>      |<span data-ttu-id="efa5a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="efa5a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="efa5a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efa5a-125">Authorization</span></span> | <span data-ttu-id="efa5a-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="efa5a-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="efa5a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efa5a-127">Request body</span></span>

<span data-ttu-id="efa5a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efa5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efa5a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="efa5a-129">Response</span></span>

<span data-ttu-id="efa5a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efa5a-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efa5a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="efa5a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efa5a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="efa5a-132">Request</span></span>

<span data-ttu-id="efa5a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efa5a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```

### <a name="response"></a><span data-ttu-id="efa5a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="efa5a-134">Response</span></span>

<span data-ttu-id="efa5a-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="efa5a-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="efa5a-136">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="efa5a-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="efa5a-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efa5a-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
