---
title: Список Макострустедрутцертификатес
description: Список свойств и связей объектов Макострустедрутцертификате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb3e9e8304e3bdd0b193c34a5da037ce41e97b4b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792753"
---
# <a name="list-macostrustedrootcertificates"></a><span data-ttu-id="1c275-103">Список Макострустедрутцертификатес</span><span class="sxs-lookup"><span data-stu-id="1c275-103">List macOSTrustedRootCertificates</span></span>

<span data-ttu-id="1c275-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c275-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c275-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c275-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c275-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c275-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c275-107">Список свойств и связей объектов [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1c275-107">List properties and relationships of the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c275-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c275-108">Prerequisites</span></span>
<span data-ttu-id="1c275-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1c275-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1c275-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c275-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c275-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c275-111">Permission type</span></span>|<span data-ttu-id="1c275-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c275-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c275-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c275-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c275-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c275-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c275-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c275-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c275-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c275-116">Not supported.</span></span>|
|<span data-ttu-id="1c275-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c275-117">Application</span></span>|<span data-ttu-id="1c275-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c275-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c275-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c275-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="1c275-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c275-120">Request headers</span></span>
|<span data-ttu-id="1c275-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c275-121">Header</span></span>|<span data-ttu-id="1c275-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c275-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c275-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c275-123">Authorization</span></span>|<span data-ttu-id="1c275-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c275-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c275-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c275-125">Accept</span></span>|<span data-ttu-id="1c275-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c275-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c275-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c275-127">Request body</span></span>
<span data-ttu-id="1c275-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c275-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c275-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c275-129">Response</span></span>
<span data-ttu-id="1c275-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c275-130">If successful, this method returns a `200 OK` response code and a collection of [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c275-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1c275-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c275-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c275-132">Request</span></span>
<span data-ttu-id="1c275-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c275-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

### <a name="response"></a><span data-ttu-id="1c275-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c275-134">Response</span></span>
<span data-ttu-id="1c275-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1c275-135">Here is an example of the response.</span></span> <span data-ttu-id="1c275-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1c275-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1c275-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1c275-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1479

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
      "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value"
    }
  ]
}
```



