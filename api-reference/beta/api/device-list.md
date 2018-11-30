---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
ms.openlocfilehash: 3e8d6b61dd9eb59e3475fa8c5d095ea649f0b9f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079785"
---
# <a name="list-devices"></a><span data-ttu-id="8cf0e-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="8cf0e-103">List devices</span></span>

> <span data-ttu-id="8cf0e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cf0e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cf0e-106">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-106">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8cf0e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cf0e-107">Permissions</span></span>
<span data-ttu-id="8cf0e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8cf0e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cf0e-110">Permission type</span></span>      | <span data-ttu-id="8cf0e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cf0e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cf0e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cf0e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cf0e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cf0e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cf0e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cf0e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cf0e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-115">Not supported.</span></span>    |
|<span data-ttu-id="8cf0e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cf0e-116">Application</span></span> | <span data-ttu-id="8cf0e-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf0e-117">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cf0e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cf0e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8cf0e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8cf0e-119">Optional query parameters</span></span>
<span data-ttu-id="8cf0e-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8cf0e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cf0e-121">Request headers</span></span>
| <span data-ttu-id="8cf0e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8cf0e-122">Name</span></span>       | <span data-ttu-id="8cf0e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8cf0e-123">Type</span></span> | <span data-ttu-id="8cf0e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8cf0e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8cf0e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cf0e-125">Authorization</span></span>  | <span data-ttu-id="8cf0e-126">string</span><span class="sxs-lookup"><span data-stu-id="8cf0e-126">string</span></span>  | <span data-ttu-id="8cf0e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cf0e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cf0e-129">Request body</span></span>
<span data-ttu-id="8cf0e-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cf0e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cf0e-131">Response</span></span>

<span data-ttu-id="8cf0e-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-132">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cf0e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8cf0e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cf0e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cf0e-134">Request</span></span>
<span data-ttu-id="8cf0e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cf0e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/beta/devices
```
##### <a name="response"></a><span data-ttu-id="8cf0e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cf0e-136">Response</span></span>
<span data-ttu-id="8cf0e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8cf0e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
