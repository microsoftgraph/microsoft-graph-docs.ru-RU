---
title: Список Андроиддевицеовнертрустедрутцертификатес
description: Список свойств и связей объектов Андроиддевицеовнертрустедрутцертификате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fed9b7de0e21b149fe7302f99715eb5b173bc17c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43349800"
---
# <a name="list-androiddeviceownertrustedrootcertificates"></a><span data-ttu-id="70ddb-103">Список Андроиддевицеовнертрустедрутцертификатес</span><span class="sxs-lookup"><span data-stu-id="70ddb-103">List androidDeviceOwnerTrustedRootCertificates</span></span>

<span data-ttu-id="70ddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70ddb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70ddb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70ddb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70ddb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70ddb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70ddb-107">Список свойств и связей объектов [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="70ddb-107">List properties and relationships of the [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70ddb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="70ddb-108">Prerequisites</span></span>
<span data-ttu-id="70ddb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70ddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70ddb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70ddb-111">Permission type</span></span>|<span data-ttu-id="70ddb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70ddb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70ddb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70ddb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70ddb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70ddb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="70ddb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70ddb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70ddb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70ddb-116">Not supported.</span></span>|
|<span data-ttu-id="70ddb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70ddb-117">Application</span></span>|<span data-ttu-id="70ddb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70ddb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70ddb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70ddb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="70ddb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="70ddb-120">Request headers</span></span>
|<span data-ttu-id="70ddb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70ddb-121">Header</span></span>|<span data-ttu-id="70ddb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="70ddb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70ddb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70ddb-123">Authorization</span></span>|<span data-ttu-id="70ddb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70ddb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70ddb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70ddb-125">Accept</span></span>|<span data-ttu-id="70ddb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70ddb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70ddb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70ddb-127">Request body</span></span>
<span data-ttu-id="70ddb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70ddb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70ddb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="70ddb-129">Response</span></span>
<span data-ttu-id="70ddb-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70ddb-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70ddb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="70ddb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="70ddb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="70ddb-132">Request</span></span>
<span data-ttu-id="70ddb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70ddb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="70ddb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70ddb-134">Response</span></span>
<span data-ttu-id="70ddb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70ddb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1492

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerTrustedRootCertificate",
      "id": "6efc1a55-1a55-6efc-551a-fc6e551afc6e",
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



