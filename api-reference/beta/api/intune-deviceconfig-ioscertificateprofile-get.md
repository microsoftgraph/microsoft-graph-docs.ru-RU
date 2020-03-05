---
title: Get iosCertificateProfile
description: Чтение свойств и связей объекта iosCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58faf460b57a25a529c3516219b9efbcb36a32a8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449070"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="e03c5-103">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e03c5-103">Get iosCertificateProfile</span></span>

<span data-ttu-id="e03c5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e03c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e03c5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e03c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e03c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e03c5-107">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e03c5-107">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e03c5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e03c5-108">Prerequisites</span></span>
<span data-ttu-id="e03c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e03c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e03c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e03c5-111">Permission type</span></span>|<span data-ttu-id="e03c5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e03c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e03c5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e03c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e03c5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e03c5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e03c5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e03c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e03c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e03c5-116">Not supported.</span></span>|
|<span data-ttu-id="e03c5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e03c5-117">Application</span></span>|<span data-ttu-id="e03c5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e03c5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e03c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e03c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeEncryptionCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e03c5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e03c5-120">Optional query parameters</span></span>
<span data-ttu-id="e03c5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e03c5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e03c5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e03c5-122">Request headers</span></span>
|<span data-ttu-id="e03c5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e03c5-123">Header</span></span>|<span data-ttu-id="e03c5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e03c5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e03c5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e03c5-125">Authorization</span></span>|<span data-ttu-id="e03c5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e03c5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e03c5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e03c5-127">Accept</span></span>|<span data-ttu-id="e03c5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e03c5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e03c5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e03c5-129">Request body</span></span>
<span data-ttu-id="e03c5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e03c5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e03c5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e03c5-131">Response</span></span>
<span data-ttu-id="e03c5-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e03c5-132">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e03c5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e03c5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e03c5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e03c5-134">Request</span></span>
<span data-ttu-id="e03c5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e03c5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="e03c5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e03c5-136">Response</span></span>
<span data-ttu-id="e03c5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e03c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1279

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
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
    "version": 7
  }
}
```





