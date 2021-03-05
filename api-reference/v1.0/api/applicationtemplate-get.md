---
title: Получение applicationTemplate
description: Получение свойств и связей объекта applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: fa9276b3dffd6ecca8df004e469c0dcd562011d9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50476446"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="b7865-103">Получение applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="b7865-103">Get applicationTemplate</span></span>

<span data-ttu-id="b7865-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7865-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7865-105">Получение свойств объекта [applicationTemplate.](../resources/applicationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="b7865-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7865-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7865-106">Permissions</span></span>

<span data-ttu-id="b7865-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7865-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7865-109">Permission type</span></span>                        | <span data-ttu-id="b7865-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7865-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b7865-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7865-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7865-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="b7865-112">None.</span></span>                                       |
| <span data-ttu-id="b7865-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7865-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7865-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7865-114">Not supported.</span></span>                              |
| <span data-ttu-id="b7865-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7865-115">Application</span></span>                            | <span data-ttu-id="b7865-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="b7865-116">None.</span></span>                                       |

<span data-ttu-id="b7865-117">Дополнительные разрешения не требуются для вызова этого API, если приложение имеет допустимый маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7865-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="b7865-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7865-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7865-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7865-119">Optional query parameters</span></span>

<span data-ttu-id="b7865-120">Параметр запроса можно указать только свойства, необходимые `$select` для лучшей производительности.</span><span class="sxs-lookup"><span data-stu-id="b7865-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="b7865-121">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="b7865-121">The **id** property is always returned.</span></span>

<span data-ttu-id="b7865-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b7865-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7865-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7865-123">Request headers</span></span>

| <span data-ttu-id="b7865-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b7865-124">Name</span></span>          | <span data-ttu-id="b7865-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b7865-125">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="b7865-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7865-126">Authorization</span></span> | <span data-ttu-id="b7865-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b7865-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7865-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7865-128">Request body</span></span>

<span data-ttu-id="b7865-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7865-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7865-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7865-130">Response</span></span>

<span data-ttu-id="b7865-131">В случае успешного применения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [applicationTemplate](../resources/applicationtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b7865-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7865-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="b7865-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b7865-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7865-133">Request</span></span>

<span data-ttu-id="b7865-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7865-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applicationTemplates/{id}
```

### <a name="response"></a><span data-ttu-id="b7865-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7865-135">Response</span></span>

<span data-ttu-id="b7865-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7865-136">The following is an example of the response.</span></span>

> <span data-ttu-id="b7865-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b7865-137">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
