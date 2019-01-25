---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: df612a24d9ffd50a432d7b6787b60de62764723c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511025"
---
# <a name="list-devices"></a><span data-ttu-id="5344e-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="5344e-103">List devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5344e-104">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="5344e-104">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5344e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5344e-105">Permissions</span></span>
<span data-ttu-id="5344e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5344e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5344e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5344e-108">Permission type</span></span>      | <span data-ttu-id="5344e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5344e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5344e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5344e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5344e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5344e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5344e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5344e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5344e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5344e-113">Not supported.</span></span>    |
|<span data-ttu-id="5344e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5344e-114">Application</span></span> | <span data-ttu-id="5344e-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5344e-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5344e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5344e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5344e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5344e-117">Optional query parameters</span></span>
<span data-ttu-id="5344e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5344e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5344e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5344e-119">Request headers</span></span>
| <span data-ttu-id="5344e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5344e-120">Name</span></span>       | <span data-ttu-id="5344e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5344e-121">Type</span></span> | <span data-ttu-id="5344e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5344e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5344e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5344e-123">Authorization</span></span>  | <span data-ttu-id="5344e-124">string</span><span class="sxs-lookup"><span data-stu-id="5344e-124">string</span></span>  | <span data-ttu-id="5344e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5344e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5344e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5344e-127">Request body</span></span>
<span data-ttu-id="5344e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5344e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5344e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5344e-129">Response</span></span>

<span data-ttu-id="5344e-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5344e-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5344e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5344e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5344e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5344e-132">Request</span></span>
<span data-ttu-id="5344e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5344e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/beta/devices
```
##### <a name="response"></a><span data-ttu-id="5344e-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5344e-134">Response</span></span>
<span data-ttu-id="5344e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5344e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/device-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
