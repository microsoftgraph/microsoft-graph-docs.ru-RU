---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2c6e452aaa237c99b39292a0fca6fd3bc760dbc
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939615"
---
# <a name="get-reportroot"></a><span data-ttu-id="5d492-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="5d492-103">Get reportRoot</span></span>

> <span data-ttu-id="5d492-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d492-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d492-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d492-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d492-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d492-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d492-107">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="5d492-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d492-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5d492-108">Prerequisites</span></span>
<span data-ttu-id="5d492-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d492-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d492-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d492-111">Permission type</span></span>|<span data-ttu-id="5d492-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d492-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d492-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d492-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5d492-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5d492-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5d492-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d492-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5d492-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="5d492-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5d492-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d492-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="5d492-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d492-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d492-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d492-119">Not supported.</span></span>|
|<span data-ttu-id="5d492-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d492-120">Application</span></span>||
| <span data-ttu-id="5d492-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="5d492-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5d492-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d492-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5d492-123">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="5d492-123">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="5d492-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d492-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d492-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d492-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d492-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5d492-126">Optional query parameters</span></span>
<span data-ttu-id="5d492-127">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5d492-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5d492-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d492-128">Request headers</span></span>
|<span data-ttu-id="5d492-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d492-129">Header</span></span>|<span data-ttu-id="5d492-130">Значение</span><span class="sxs-lookup"><span data-stu-id="5d492-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d492-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d492-131">Authorization</span></span>|<span data-ttu-id="5d492-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d492-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d492-133">Accept</span><span class="sxs-lookup"><span data-stu-id="5d492-133">Accept</span></span>|<span data-ttu-id="5d492-134">application/json</span><span class="sxs-lookup"><span data-stu-id="5d492-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d492-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d492-135">Request body</span></span>
<span data-ttu-id="5d492-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d492-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d492-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d492-137">Response</span></span>
<span data-ttu-id="5d492-138">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5d492-138">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d492-139">Пример</span><span class="sxs-lookup"><span data-stu-id="5d492-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d492-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d492-140">Request</span></span>
<span data-ttu-id="5d492-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d492-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="5d492-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d492-142">Response</span></span>
<span data-ttu-id="5d492-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d492-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











