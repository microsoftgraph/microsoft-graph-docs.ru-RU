---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 98339a50b4d0422f6392cf193f1b4c2377e7f515
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950461"
---
# <a name="get-reportroot"></a><span data-ttu-id="81f6a-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="81f6a-103">Get reportRoot</span></span>

> <span data-ttu-id="81f6a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81f6a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81f6a-105">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="81f6a-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81f6a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="81f6a-106">Prerequisites</span></span>
<span data-ttu-id="81f6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81f6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81f6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81f6a-109">Permission type</span></span>|<span data-ttu-id="81f6a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81f6a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81f6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81f6a-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="81f6a-112">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="81f6a-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="81f6a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81f6a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="81f6a-114">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="81f6a-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="81f6a-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="81f6a-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="81f6a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81f6a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81f6a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81f6a-117">Not supported.</span></span>|
|<span data-ttu-id="81f6a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81f6a-118">Application</span></span>|<span data-ttu-id="81f6a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81f6a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81f6a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81f6a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81f6a-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81f6a-121">Optional query parameters</span></span>
<span data-ttu-id="81f6a-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81f6a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="81f6a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81f6a-123">Request headers</span></span>
|<span data-ttu-id="81f6a-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81f6a-124">Header</span></span>|<span data-ttu-id="81f6a-125">Значение</span><span class="sxs-lookup"><span data-stu-id="81f6a-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81f6a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="81f6a-126">Authorization</span></span>|<span data-ttu-id="81f6a-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="81f6a-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81f6a-128">Accept</span><span class="sxs-lookup"><span data-stu-id="81f6a-128">Accept</span></span>|<span data-ttu-id="81f6a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="81f6a-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81f6a-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81f6a-130">Request body</span></span>
<span data-ttu-id="81f6a-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81f6a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81f6a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="81f6a-132">Response</span></span>
<span data-ttu-id="81f6a-133">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="81f6a-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81f6a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="81f6a-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="81f6a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="81f6a-135">Request</span></span>
<span data-ttu-id="81f6a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81f6a-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="81f6a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="81f6a-137">Response</span></span>
<span data-ttu-id="81f6a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="81f6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```








