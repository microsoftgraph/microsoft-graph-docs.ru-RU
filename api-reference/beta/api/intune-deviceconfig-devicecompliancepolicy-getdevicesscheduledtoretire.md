---
title: действие Жетдевицессчедуледторетире
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adf98b4a1703a0e84f15dc0a310677d37bd9e124
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292445"
---
# <a name="getdevicesscheduledtoretire-action"></a><span data-ttu-id="a89ba-103">действие Жетдевицессчедуледторетире</span><span class="sxs-lookup"><span data-stu-id="a89ba-103">getDevicesScheduledToRetire action</span></span>

<span data-ttu-id="a89ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a89ba-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a89ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a89ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a89ba-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a89ba-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a89ba-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a89ba-108">Prerequisites</span></span>
<span data-ttu-id="a89ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a89ba-111">Permission type</span></span>|<span data-ttu-id="a89ba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a89ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a89ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a89ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a89ba-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a89ba-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a89ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a89ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a89ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89ba-116">Not supported.</span></span>|
|<span data-ttu-id="a89ba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a89ba-117">Application</span></span>|<span data-ttu-id="a89ba-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a89ba-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a89ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a89ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

## <a name="request-headers"></a><span data-ttu-id="a89ba-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a89ba-120">Request headers</span></span>
|<span data-ttu-id="a89ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a89ba-121">Header</span></span>|<span data-ttu-id="a89ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a89ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a89ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a89ba-123">Authorization</span></span>|<span data-ttu-id="a89ba-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a89ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a89ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a89ba-125">Accept</span></span>|<span data-ttu-id="a89ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a89ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a89ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a89ba-127">Request body</span></span>
<span data-ttu-id="a89ba-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a89ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89ba-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89ba-129">Response</span></span>
<span data-ttu-id="a89ba-130">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [ретиресчедуледманажеддевице](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a89ba-130">If successful, this action returns a `200 OK` response code and a [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a89ba-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a89ba-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a89ba-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a89ba-132">Request</span></span>
<span data-ttu-id="a89ba-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a89ba-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

### <a name="response"></a><span data-ttu-id="a89ba-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89ba-134">Response</span></span>
<span data-ttu-id="a89ba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a89ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 670

{
  "value": [
    {
      "@odata.type": "microsoft.graph.retireScheduledManagedDevice",
      "id": "Id value",
      "managedDeviceId": "Managed Device Id value",
      "managedDeviceName": "Managed Device Name value",
      "deviceType": "windowsRT",
      "complianceState": "notApplicable",
      "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
      "managementAgent": "mdm",
      "ownerType": "company",
      "deviceCompliancePolicyName": "Device Compliance Policy Name value",
      "deviceCompliancePolicyId": "Device Compliance Policy Id value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




