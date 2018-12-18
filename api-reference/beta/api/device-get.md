---
title: Получение устройства
description: Получение свойств и связей объекта устройства.
author: tfitzmac
ms.openlocfilehash: 632094db64cce86a965751d97b0ae9c92d439d5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348267"
---
# <a name="get-device"></a><span data-ttu-id="dfbe7-103">Получение устройства</span><span class="sxs-lookup"><span data-stu-id="dfbe7-103">Get device</span></span>

> <span data-ttu-id="dfbe7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfbe7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfbe7-106">Получение свойств и связей объекта устройства.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-106">Get the properties and relationships of a device object.</span></span>

<span data-ttu-id="dfbe7-107">Поскольку ресурсов **устройство** поддерживает [расширения](/graph/extensibility-overview), вы также можете использовать `GET` операции для получения данных расширения и настраиваемых свойств в экземпляре **устройства** .</span><span class="sxs-lookup"><span data-stu-id="dfbe7-107">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **device** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfbe7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfbe7-108">Permissions</span></span>
<span data-ttu-id="dfbe7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfbe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dfbe7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfbe7-111">Permission type</span></span>      | <span data-ttu-id="dfbe7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfbe7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfbe7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfbe7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dfbe7-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfbe7-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfbe7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfbe7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfbe7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-116">Not supported.</span></span>    |
|<span data-ttu-id="dfbe7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfbe7-117">Application</span></span> | <span data-ttu-id="dfbe7-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbe7-118">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfbe7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfbe7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dfbe7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfbe7-120">Optional query parameters</span></span>
<span data-ttu-id="dfbe7-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dfbe7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfbe7-122">Request headers</span></span>
| <span data-ttu-id="dfbe7-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dfbe7-123">Name</span></span>       | <span data-ttu-id="dfbe7-124">Тип</span><span class="sxs-lookup"><span data-stu-id="dfbe7-124">Type</span></span> | <span data-ttu-id="dfbe7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="dfbe7-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dfbe7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfbe7-126">Authorization</span></span>  | <span data-ttu-id="dfbe7-127">string</span><span class="sxs-lookup"><span data-stu-id="dfbe7-127">string</span></span>  | <span data-ttu-id="dfbe7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfbe7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfbe7-130">Request body</span></span>
<span data-ttu-id="dfbe7-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfbe7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfbe7-132">Response</span></span>

<span data-ttu-id="dfbe7-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-133">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfbe7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dfbe7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfbe7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfbe7-135">Request</span></span>
<span data-ttu-id="dfbe7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}
```

> <span data-ttu-id="dfbe7-137">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-137">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

##### <a name="response"></a><span data-ttu-id="dfbe7-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfbe7-138">Response</span></span>
<span data-ttu-id="dfbe7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dfbe7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dfbe7-142">См. также</span><span class="sxs-lookup"><span data-stu-id="dfbe7-142">See also</span></span>

- [<span data-ttu-id="dfbe7-143">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="dfbe7-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="dfbe7-144">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="dfbe7-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="dfbe7-145">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="dfbe7-145">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->