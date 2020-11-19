---
title: List deviceComplianceDeviceStatuses
description: Перечисление свойств и связей объектов deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99bb7fb05856dbb65c45de2739d04a066357433a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292466"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="307f2-103">List deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="307f2-103">List deviceComplianceDeviceStatuses</span></span>

<span data-ttu-id="307f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="307f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="307f2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="307f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="307f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="307f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="307f2-107">Перечисление свойств и связей объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="307f2-107">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="307f2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="307f2-108">Prerequisites</span></span>
<span data-ttu-id="307f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="307f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="307f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="307f2-111">Permission type</span></span>|<span data-ttu-id="307f2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="307f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="307f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="307f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="307f2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="307f2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="307f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="307f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="307f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="307f2-116">Not supported.</span></span>|
|<span data-ttu-id="307f2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="307f2-117">Application</span></span>|<span data-ttu-id="307f2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="307f2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="307f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="307f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="307f2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="307f2-120">Request headers</span></span>
|<span data-ttu-id="307f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="307f2-121">Header</span></span>|<span data-ttu-id="307f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="307f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="307f2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="307f2-123">Authorization</span></span>|<span data-ttu-id="307f2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="307f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="307f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="307f2-125">Accept</span></span>|<span data-ttu-id="307f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="307f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="307f2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="307f2-127">Request body</span></span>
<span data-ttu-id="307f2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="307f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="307f2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="307f2-129">Response</span></span>
<span data-ttu-id="307f2-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="307f2-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="307f2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="307f2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="307f2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="307f2-132">Request</span></span>
<span data-ttu-id="307f2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="307f2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="307f2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="307f2-134">Response</span></span>
<span data-ttu-id="307f2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="307f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
      "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




