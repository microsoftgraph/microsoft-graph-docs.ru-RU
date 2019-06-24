---
title: Список Аппликатионтемплатес
description: Получение списка объектов аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac8ad3a8b4a7a396c0cb35c1c72c2d1a2e309184
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147933"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="84bb6-103">Список Аппликатионтемплатес</span><span class="sxs-lookup"><span data-stu-id="84bb6-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84bb6-104">Получение списка объектов [аппликатионтемплате](../resources/applicationtemplate.md) из коллекции приложений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84bb6-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="84bb6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84bb6-105">Permissions</span></span>

<span data-ttu-id="84bb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84bb6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84bb6-108">Permission type</span></span>                        | <span data-ttu-id="84bb6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84bb6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84bb6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84bb6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="84bb6-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="84bb6-111">None.</span></span> |
| <span data-ttu-id="84bb6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84bb6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84bb6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84bb6-113">Not supported.</span></span> |
| <span data-ttu-id="84bb6-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="84bb6-114">Application</span></span>                            | <span data-ttu-id="84bb6-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84bb6-115">None.</span></span> |

<span data-ttu-id="84bb6-116">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="84bb6-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="84bb6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84bb6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84bb6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84bb6-118">Optional query parameters</span></span>

<span data-ttu-id="84bb6-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84bb6-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="84bb6-120">Вы можете использовать этот `$filter` параметр ограниченное количеством способов.</span><span class="sxs-lookup"><span data-stu-id="84bb6-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="84bb6-121">Фильтровать можно только по **DisplayName** или **категориям**.</span><span class="sxs-lookup"><span data-stu-id="84bb6-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="84bb6-122">Пример:  `$filter=contains(displayName, 'salesf')` или `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="84bb6-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="84bb6-123">Вы можете использовать `$orderby` `$top,` и `$skip` запрос параметров в любом запросе GET.</span><span class="sxs-lookup"><span data-stu-id="84bb6-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="84bb6-124">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="84bb6-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="84bb6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84bb6-125">Request headers</span></span>

| <span data-ttu-id="84bb6-126">Имя</span><span class="sxs-lookup"><span data-stu-id="84bb6-126">Name</span></span>      |<span data-ttu-id="84bb6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="84bb6-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84bb6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84bb6-128">Authorization</span></span> | <span data-ttu-id="84bb6-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="84bb6-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="84bb6-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84bb6-130">Request body</span></span>

<span data-ttu-id="84bb6-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84bb6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84bb6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="84bb6-132">Response</span></span>

<span data-ttu-id="84bb6-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84bb6-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84bb6-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="84bb6-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84bb6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="84bb6-135">Request</span></span>

<span data-ttu-id="84bb6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84bb6-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates
```

### <a name="response"></a><span data-ttu-id="84bb6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="84bb6-137">Response</span></span>

<span data-ttu-id="84bb6-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84bb6-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="84bb6-139">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84bb6-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="84bb6-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84bb6-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applicationTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
