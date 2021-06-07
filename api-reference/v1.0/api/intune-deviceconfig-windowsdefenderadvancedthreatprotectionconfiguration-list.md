---
title: Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration
description: Список свойств и связей объектов windowsDefenderAdvancedThreatProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8721cf8435653aff733390a383d515c477d25975
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747223"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="9cff9-103">Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="9cff9-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

<span data-ttu-id="9cff9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cff9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cff9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cff9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cff9-106">Список свойств и связей объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9cff9-106">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cff9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9cff9-107">Prerequisites</span></span>
<span data-ttu-id="9cff9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cff9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cff9-110">Permission type</span></span>|<span data-ttu-id="9cff9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cff9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cff9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cff9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9cff9-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cff9-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cff9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cff9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cff9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cff9-115">Not supported.</span></span>|
|<span data-ttu-id="9cff9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9cff9-116">Application</span></span>|<span data-ttu-id="9cff9-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cff9-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cff9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cff9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9cff9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9cff9-119">Request headers</span></span>
|<span data-ttu-id="9cff9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cff9-120">Header</span></span>|<span data-ttu-id="9cff9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9cff9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cff9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cff9-122">Authorization</span></span>|<span data-ttu-id="9cff9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cff9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cff9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9cff9-124">Accept</span></span>|<span data-ttu-id="9cff9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9cff9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cff9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cff9-126">Request body</span></span>
<span data-ttu-id="9cff9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9cff9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cff9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cff9-128">Response</span></span>
<span data-ttu-id="9cff9-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9cff9-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cff9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9cff9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cff9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cff9-131">Request</span></span>
<span data-ttu-id="9cff9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cff9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9cff9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cff9-133">Response</span></span>
<span data-ttu-id="9cff9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cff9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
      "id": "294373aa-73aa-2943-aa73-4329aa734329",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "allowSampleSharing": true,
      "enableExpeditedTelemetryReporting": true
    }
  ]
}
```




