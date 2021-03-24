---
title: Get comanagementEligibleDevice
description: Чтение свойств и связей объекта comanagementEligibleDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a172735c64d6003d2db08065cbeff532546f7e3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128658"
---
# <a name="get-comanagementeligibledevice"></a><span data-ttu-id="b51e4-103">Get comanagementEligibleDevice</span><span class="sxs-lookup"><span data-stu-id="b51e4-103">Get comanagementEligibleDevice</span></span>

<span data-ttu-id="b51e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b51e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b51e4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b51e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b51e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b51e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b51e4-107">Чтение свойств и связей [объекта comanagementEligibleDevice.](../resources/intune-devices-comanagementeligibledevice.md)</span><span class="sxs-lookup"><span data-stu-id="b51e4-107">Read properties and relationships of the [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b51e4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b51e4-108">Prerequisites</span></span>
<span data-ttu-id="b51e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b51e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b51e4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b51e4-111">Permission type</span></span>|<span data-ttu-id="b51e4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b51e4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b51e4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b51e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b51e4-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b51e4-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b51e4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b51e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b51e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b51e4-116">Not supported.</span></span>|
|<span data-ttu-id="b51e4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b51e4-117">Application</span></span>|<span data-ttu-id="b51e4-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b51e4-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b51e4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b51e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b51e4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b51e4-120">Optional query parameters</span></span>
<span data-ttu-id="b51e4-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b51e4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b51e4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b51e4-122">Request headers</span></span>
|<span data-ttu-id="b51e4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b51e4-123">Header</span></span>|<span data-ttu-id="b51e4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b51e4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b51e4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b51e4-125">Authorization</span></span>|<span data-ttu-id="b51e4-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b51e4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b51e4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b51e4-127">Accept</span></span>|<span data-ttu-id="b51e4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b51e4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b51e4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b51e4-129">Request body</span></span>
<span data-ttu-id="b51e4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b51e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b51e4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b51e4-131">Response</span></span>
<span data-ttu-id="b51e4-132">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b51e4-132">If successful, this method returns a `200 OK` response code and [comanagementEligibleDevice](../resources/intune-devices-comanagementeligibledevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b51e4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b51e4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b51e4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b51e4-134">Request</span></span>
<span data-ttu-id="b51e4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b51e4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

### <a name="response"></a><span data-ttu-id="b51e4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b51e4-136">Response</span></span>
<span data-ttu-id="b51e4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b51e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 824

{
  "value": {
    "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
    "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
    "deviceName": "Device Name value",
    "deviceType": "windowsRT",
    "clientRegistrationStatus": "registered",
    "ownerType": "company",
    "managementAgents": "mdm",
    "managementState": "retirePending",
    "referenceId": "Reference Id value",
    "mdmStatus": "Mdm Status value",
    "osVersion": "Os Version value",
    "serialNumber": "Serial Number value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "osDescription": "Os Description value",
    "entitySource": 12,
    "userId": "User Id value",
    "upn": "Upn value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "status": "eligible"
  }
}
```




