---
title: Получение устройства
description: Получение свойств и связей объекта устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e52d339b4be3af43ab6d1c3e5cb6f30bc16c262e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435887"
---
# <a name="get-device"></a><span data-ttu-id="08ab8-103">Вывод устройства</span><span class="sxs-lookup"><span data-stu-id="08ab8-103">Get device</span></span>

<span data-ttu-id="08ab8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08ab8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08ab8-105">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="08ab8-105">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="08ab8-106">Так как ресурс **Device** поддерживает [расширения](/graph/extensibility-overview), с помощью `GET` операции можно также получить настраиваемые свойства и данные расширения в экземпляре **устройства** .</span><span class="sxs-lookup"><span data-stu-id="08ab8-106">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="08ab8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08ab8-107">Permissions</span></span>
<span data-ttu-id="08ab8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ab8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="08ab8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08ab8-110">Permission type</span></span>      | <span data-ttu-id="08ab8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08ab8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08ab8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08ab8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08ab8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08ab8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08ab8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08ab8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08ab8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ab8-115">Not supported.</span></span>    |
|<span data-ttu-id="08ab8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08ab8-116">Application</span></span> | <span data-ttu-id="08ab8-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08ab8-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08ab8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08ab8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08ab8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08ab8-119">Optional query parameters</span></span>
<span data-ttu-id="08ab8-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08ab8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="08ab8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08ab8-121">Request headers</span></span>
| <span data-ttu-id="08ab8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="08ab8-122">Name</span></span>       | <span data-ttu-id="08ab8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="08ab8-123">Type</span></span> | <span data-ttu-id="08ab8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="08ab8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="08ab8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08ab8-125">Authorization</span></span>  | <span data-ttu-id="08ab8-126">string</span><span class="sxs-lookup"><span data-stu-id="08ab8-126">string</span></span>  | <span data-ttu-id="08ab8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08ab8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08ab8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08ab8-129">Request body</span></span>
<span data-ttu-id="08ab8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08ab8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ab8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="08ab8-131">Response</span></span>

<span data-ttu-id="08ab8-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08ab8-132">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08ab8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="08ab8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08ab8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="08ab8-134">Request</span></span>
<span data-ttu-id="08ab8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08ab8-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08ab8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="08ab8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="08ab8-137">C#</span><span class="sxs-lookup"><span data-stu-id="08ab8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08ab8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08ab8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08ab8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08ab8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


> <span data-ttu-id="08ab8-140">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="08ab8-140">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="08ab8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="08ab8-141">Response</span></span>
<span data-ttu-id="08ab8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="08ab8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "deviceVersion": 99
}
```

## <a name="see-also"></a><span data-ttu-id="08ab8-145">См. также</span><span class="sxs-lookup"><span data-stu-id="08ab8-145">See also</span></span>

- [<span data-ttu-id="08ab8-146">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="08ab8-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="08ab8-147">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="08ab8-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="08ab8-148">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="08ab8-148">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
