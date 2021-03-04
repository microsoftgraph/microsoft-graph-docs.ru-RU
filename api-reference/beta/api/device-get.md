---
title: Получение устройства
description: Получение свойств и связей объекта устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8c1c70578ed95ead160895e5d471a8c4ba56e6c8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437207"
---
# <a name="get-device"></a><span data-ttu-id="87c76-103">Вывод устройства</span><span class="sxs-lookup"><span data-stu-id="87c76-103">Get device</span></span>

<span data-ttu-id="87c76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87c76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87c76-105">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="87c76-105">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="87c76-106">Так как **ресурс устройства** поддерживает [расширения,](/graph/extensibility-overview)вы также можете использовать операцию для получения настраиваемой информации о свойствах и расширении в `GET` **экземпляре** устройства.</span><span class="sxs-lookup"><span data-stu-id="87c76-106">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="87c76-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87c76-107">Permissions</span></span>
<span data-ttu-id="87c76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87c76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87c76-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87c76-110">Permission type</span></span>      | <span data-ttu-id="87c76-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87c76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c76-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87c76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87c76-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="87c76-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87c76-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87c76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87c76-115">Not supported.</span></span>    |
|<span data-ttu-id="87c76-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="87c76-116">Application</span></span> | <span data-ttu-id="87c76-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87c76-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87c76-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87c76-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87c76-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="87c76-119">Optional query parameters</span></span>
<span data-ttu-id="87c76-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="87c76-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87c76-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87c76-121">Request headers</span></span>
| <span data-ttu-id="87c76-122">Имя</span><span class="sxs-lookup"><span data-stu-id="87c76-122">Name</span></span>       | <span data-ttu-id="87c76-123">Тип</span><span class="sxs-lookup"><span data-stu-id="87c76-123">Type</span></span> | <span data-ttu-id="87c76-124">Описание</span><span class="sxs-lookup"><span data-stu-id="87c76-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="87c76-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="87c76-125">Authorization</span></span>  | <span data-ttu-id="87c76-126">string</span><span class="sxs-lookup"><span data-stu-id="87c76-126">string</span></span>  | <span data-ttu-id="87c76-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87c76-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87c76-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87c76-129">Request body</span></span>
<span data-ttu-id="87c76-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87c76-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87c76-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="87c76-131">Response</span></span>

<span data-ttu-id="87c76-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87c76-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87c76-133">Пример</span><span class="sxs-lookup"><span data-stu-id="87c76-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="87c76-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="87c76-134">Request</span></span>
<span data-ttu-id="87c76-135">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87c76-135">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87c76-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="87c76-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="87c76-137">C#</span><span class="sxs-lookup"><span data-stu-id="87c76-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87c76-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87c76-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87c76-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87c76-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87c76-140">Java</span><span class="sxs-lookup"><span data-stu-id="87c76-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="87c76-141">**Примечание:** В `id` запросе находится свойство **id** устройства, а не **свойство deviceId.**</span><span class="sxs-lookup"><span data-stu-id="87c76-141">**Note:** The `id` in the request is the **id** property of the device, not the **deviceId** property.</span></span>

### <a name="response"></a><span data-ttu-id="87c76-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="87c76-142">Response</span></span>
<span data-ttu-id="87c76-143">В следующем примере показан ответ на устройство без **имен hostNames.**</span><span class="sxs-lookup"><span data-stu-id="87c76-143">The following example shows a response for a device with no **hostNames**.</span></span> 

><span data-ttu-id="87c76-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="87c76-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 322

{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99,
  "hostNames": []
}
```

<span data-ttu-id="87c76-145">В следующем примере показан ответ на устройство с **именами hostNames.**</span><span class="sxs-lookup"><span data-stu-id="87c76-145">The following example shows a response for a device with **hostNames**.</span></span> 

><span data-ttu-id="87c76-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="87c76-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 322

{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
  "deviceId": "deviceId-value",
  "deviceMetadata": "deviceMetadata-value",
  "deviceVersion": 99,
  "hostnames":["hostname1.contoso.onmicrosoft.com", "hostname1"]
}
```


## <a name="see-also"></a><span data-ttu-id="87c76-147">См. также</span><span class="sxs-lookup"><span data-stu-id="87c76-147">See also</span></span>

- [<span data-ttu-id="87c76-148">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="87c76-148">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="87c76-149">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="87c76-149">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="87c76-150">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="87c76-150">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
