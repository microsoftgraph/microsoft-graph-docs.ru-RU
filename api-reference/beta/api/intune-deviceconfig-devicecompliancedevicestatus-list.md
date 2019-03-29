---
title: List deviceComplianceDeviceStatuses
description: Перечисление свойств и связей объектов deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01c9427b26a7088513581af1e5b27ef91abdf673
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969808"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="6be1f-103">List deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6be1f-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="6be1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be1f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6be1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be1f-106">Перечисление свойств и связей объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6be1f-106">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6be1f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6be1f-107">Prerequisites</span></span>
<span data-ttu-id="6be1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6be1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6be1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6be1f-110">Permission type</span></span>|<span data-ttu-id="6be1f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6be1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6be1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6be1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6be1f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6be1f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6be1f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6be1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6be1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be1f-115">Not supported.</span></span>|
|<span data-ttu-id="6be1f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6be1f-116">Application</span></span>|<span data-ttu-id="6be1f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6be1f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6be1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6be1f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6be1f-119">Request headers</span></span>
|<span data-ttu-id="6be1f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6be1f-120">Header</span></span>|<span data-ttu-id="6be1f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6be1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6be1f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6be1f-122">Authorization</span></span>|<span data-ttu-id="6be1f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6be1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6be1f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6be1f-124">Accept</span></span>|<span data-ttu-id="6be1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6be1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6be1f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6be1f-126">Request body</span></span>
<span data-ttu-id="6be1f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6be1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6be1f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6be1f-128">Response</span></span>
<span data-ttu-id="6be1f-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6be1f-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6be1f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6be1f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6be1f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6be1f-131">Request</span></span>
<span data-ttu-id="6be1f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6be1f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="6be1f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6be1f-133">Response</span></span>
<span data-ttu-id="6be1f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6be1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




