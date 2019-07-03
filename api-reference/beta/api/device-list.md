---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eec732d08a18158570f6826bb9b06208f8d4d4dd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437224"
---
# <a name="list-devices"></a><span data-ttu-id="96b3a-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="96b3a-103">List devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96b3a-104">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="96b3a-104">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="96b3a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96b3a-105">Permissions</span></span>
<span data-ttu-id="96b3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96b3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="96b3a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96b3a-108">Permission type</span></span>      | <span data-ttu-id="96b3a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96b3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96b3a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96b3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96b3a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96b3a-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="96b3a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96b3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96b3a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96b3a-113">Not supported.</span></span>    |
|<span data-ttu-id="96b3a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96b3a-114">Application</span></span> | <span data-ttu-id="96b3a-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96b3a-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96b3a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96b3a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96b3a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96b3a-117">Optional query parameters</span></span>
<span data-ttu-id="96b3a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="96b3a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96b3a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96b3a-119">Request headers</span></span>
| <span data-ttu-id="96b3a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="96b3a-120">Name</span></span>       | <span data-ttu-id="96b3a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="96b3a-121">Type</span></span> | <span data-ttu-id="96b3a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="96b3a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96b3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96b3a-123">Authorization</span></span>  | <span data-ttu-id="96b3a-124">string</span><span class="sxs-lookup"><span data-stu-id="96b3a-124">string</span></span>  | <span data-ttu-id="96b3a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96b3a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96b3a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96b3a-127">Request body</span></span>
<span data-ttu-id="96b3a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96b3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96b3a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="96b3a-129">Response</span></span>

<span data-ttu-id="96b3a-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96b3a-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96b3a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="96b3a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96b3a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96b3a-132">Request</span></span>
<span data-ttu-id="96b3a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96b3a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96b3a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96b3a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/beta/devices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96b3a-135">C#</span><span class="sxs-lookup"><span data-stu-id="96b3a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96b3a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="96b3a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96b3a-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="96b3a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96b3a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="96b3a-138">Response</span></span>
<span data-ttu-id="96b3a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96b3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled": true,
      "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
      "deviceId": "deviceId-value",
      "deviceMetadata": "deviceMetadata-value",
      "displayName" : "displayName-value",
      "id" : "id-value", 
      "operatingSystem" : "operatingSystem-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
