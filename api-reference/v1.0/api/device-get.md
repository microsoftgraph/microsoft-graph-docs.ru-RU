---
title: Получение устройства
description: Получение свойств и связей объекта устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1454c99ae6c868fddc047ab40a5b3cf09a246f24
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276393"
---
# <a name="get-device"></a><span data-ttu-id="068a6-103">Получение устройства</span><span class="sxs-lookup"><span data-stu-id="068a6-103">Get device</span></span>

<span data-ttu-id="068a6-104">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="068a6-104">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="068a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="068a6-105">Permissions</span></span>
<span data-ttu-id="068a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="068a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="068a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="068a6-108">Permission type</span></span>      | <span data-ttu-id="068a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="068a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="068a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="068a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="068a6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="068a6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="068a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="068a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="068a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="068a6-113">Not supported.</span></span>    |
|<span data-ttu-id="068a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="068a6-114">Application</span></span> | <span data-ttu-id="068a6-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="068a6-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="068a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="068a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="068a6-117">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="068a6-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="068a6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="068a6-118">Optional query parameters</span></span>
<span data-ttu-id="068a6-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="068a6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="068a6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="068a6-120">Request headers</span></span>
| <span data-ttu-id="068a6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="068a6-121">Name</span></span>       | <span data-ttu-id="068a6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="068a6-122">Type</span></span> | <span data-ttu-id="068a6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="068a6-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="068a6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="068a6-124">Authorization</span></span>  | <span data-ttu-id="068a6-125">string</span><span class="sxs-lookup"><span data-stu-id="068a6-125">string</span></span>  | <span data-ttu-id="068a6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="068a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="068a6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="068a6-128">Request body</span></span>
<span data-ttu-id="068a6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="068a6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="068a6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="068a6-130">Response</span></span>

<span data-ttu-id="068a6-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="068a6-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="068a6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="068a6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="068a6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="068a6-133">Request</span></span>
<span data-ttu-id="068a6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="068a6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="068a6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="068a6-135">Response</span></span>
<span data-ttu-id="068a6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="068a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  "displayName":"Test device",
  "id": "id-value",
  "operatingSystem":"linux",
  "operatingSystemVersion":"1"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="068a6-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="068a6-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="068a6-140">C#</span><span class="sxs-lookup"><span data-stu-id="068a6-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="068a6-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="068a6-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_device-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="068a6-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="068a6-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_device-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
