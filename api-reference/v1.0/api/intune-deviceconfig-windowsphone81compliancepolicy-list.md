---
title: Перечисление объектов windowsPhone81CompliancePolicy
description: Список свойств и связей объектов windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d3914fe4cabaec221330cdedc1a2626354b6769
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752653"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="d0670-103">Перечисление объектов windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d0670-103">List windowsPhone81CompliancePolicies</span></span>

<span data-ttu-id="d0670-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0670-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0670-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0670-106">Список свойств и связей объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d0670-106">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0670-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0670-107">Prerequisites</span></span>
<span data-ttu-id="d0670-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0670-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0670-110">Permission type</span></span>|<span data-ttu-id="d0670-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0670-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0670-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0670-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0670-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0670-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0670-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0670-115">Not supported.</span></span>|
|<span data-ttu-id="d0670-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0670-116">Application</span></span>|<span data-ttu-id="d0670-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0670-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0670-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d0670-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0670-119">Request headers</span></span>
|<span data-ttu-id="d0670-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0670-120">Header</span></span>|<span data-ttu-id="d0670-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0670-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0670-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0670-122">Authorization</span></span>|<span data-ttu-id="d0670-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0670-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0670-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d0670-124">Accept</span></span>|<span data-ttu-id="d0670-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0670-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0670-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0670-126">Request body</span></span>
<span data-ttu-id="d0670-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0670-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0670-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0670-128">Response</span></span>
<span data-ttu-id="d0670-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0670-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0670-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d0670-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0670-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0670-131">Request</span></span>
<span data-ttu-id="d0670-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0670-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="d0670-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0670-133">Response</span></span>
<span data-ttu-id="d0670-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0670-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
      "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```




