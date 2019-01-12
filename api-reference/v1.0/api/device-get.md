---
title: Получение устройства
description: Получение свойств и связей объекта устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 110453fde3545128bb75c840e831959e31f971d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972742"
---
# <a name="get-device"></a><span data-ttu-id="4172c-103">Получение устройства</span><span class="sxs-lookup"><span data-stu-id="4172c-103">Get device</span></span>

<span data-ttu-id="4172c-104">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="4172c-104">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4172c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4172c-105">Permissions</span></span>
<span data-ttu-id="4172c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4172c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4172c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4172c-108">Permission type</span></span>      | <span data-ttu-id="4172c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4172c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4172c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4172c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4172c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4172c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4172c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4172c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4172c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4172c-113">Not supported.</span></span>    |
|<span data-ttu-id="4172c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4172c-114">Application</span></span> | <span data-ttu-id="4172c-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4172c-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4172c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4172c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="4172c-117">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="4172c-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4172c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4172c-118">Optional query parameters</span></span>
<span data-ttu-id="4172c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4172c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4172c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4172c-120">Request headers</span></span>
| <span data-ttu-id="4172c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4172c-121">Name</span></span>       | <span data-ttu-id="4172c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4172c-122">Type</span></span> | <span data-ttu-id="4172c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4172c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4172c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4172c-124">Authorization</span></span>  | <span data-ttu-id="4172c-125">string</span><span class="sxs-lookup"><span data-stu-id="4172c-125">string</span></span>  | <span data-ttu-id="4172c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4172c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4172c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4172c-128">Request body</span></span>
<span data-ttu-id="4172c-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4172c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4172c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4172c-130">Response</span></span>

<span data-ttu-id="4172c-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4172c-131">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4172c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4172c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4172c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4172c-133">Request</span></span>
<span data-ttu-id="4172c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4172c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="4172c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="4172c-135">Response</span></span>
<span data-ttu-id="4172c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4172c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
