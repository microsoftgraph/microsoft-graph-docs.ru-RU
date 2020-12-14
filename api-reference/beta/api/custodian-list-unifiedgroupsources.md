---
title: Список unifiedGroupSources
description: Получите список объектов unifiedGroupSource и их свойств.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f0bb4e23ce089001b6cec2d610ec2cb6ca0e33bb
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659121"
---
# <a name="list-unifiedgroupsources"></a><span data-ttu-id="7fed9-103">Список unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="7fed9-103">List unifiedGroupSources</span></span>

<span data-ttu-id="7fed9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fed9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fed9-105">Получите список объектов [unifiedGroupSource](../resources/unifiedgroupsource.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="7fed9-105">Get a list of the [unifiedGroupSource](../resources/unifiedgroupsource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fed9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fed9-106">Permissions</span></span>

<span data-ttu-id="7fed9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fed9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fed9-109">Permission type</span></span>|<span data-ttu-id="7fed9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fed9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fed9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fed9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7fed9-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="7fed9-112">User.Read</span></span>|
|<span data-ttu-id="7fed9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fed9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fed9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fed9-114">Not supported.</span></span>|
|<span data-ttu-id="7fed9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fed9-115">Application</span></span>|<span data-ttu-id="7fed9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fed9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fed9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fed9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fed9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7fed9-118">Optional query parameters</span></span>

<span data-ttu-id="7fed9-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7fed9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7fed9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7fed9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fed9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fed9-121">Request headers</span></span>

|<span data-ttu-id="7fed9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7fed9-122">Name</span></span>|<span data-ttu-id="7fed9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7fed9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7fed9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fed9-124">Authorization</span></span>|<span data-ttu-id="7fed9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fed9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fed9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fed9-127">Request body</span></span>

<span data-ttu-id="7fed9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fed9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fed9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fed9-129">Response</span></span>

<span data-ttu-id="7fed9-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [unifiedGroupSource](../resources/unifiedgroupsource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fed9-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedGroupSource](../resources/unifiedgroupsource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fed9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7fed9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7fed9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fed9-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7fed9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fed9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedgroupsource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```
# <a name="c"></a>[<span data-ttu-id="7fed9-134">C#</span><span class="sxs-lookup"><span data-stu-id="7fed9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedgroupsource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fed9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fed9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedgroupsource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fed9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fed9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedgroupsource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fed9-137">Java</span><span class="sxs-lookup"><span data-stu-id="7fed9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedgroupsource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fed9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fed9-138">Response</span></span>

<span data-ttu-id="7fed9-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7fed9-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedGroupSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": "Megan Bowen"
                }
            }
        }
    ]
}
```
