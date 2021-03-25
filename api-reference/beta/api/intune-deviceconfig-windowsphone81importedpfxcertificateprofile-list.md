---
title: Список windowsPhone81ImportedPFXCertificateProfiles
description: Список свойств и связей объектов WindowsPhone81ImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5db6cbc47b669f19e807c05148b10f829e1e96b1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154779"
---
# <a name="list-windowsphone81importedpfxcertificateprofiles"></a><span data-ttu-id="d70d6-103">Список windowsPhone81ImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="d70d6-103">List windowsPhone81ImportedPFXCertificateProfiles</span></span>

<span data-ttu-id="d70d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d70d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d70d6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d70d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d70d6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d70d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d70d6-107">Список свойств и связей [объектов WindowsPhone81ImportedPFXCertificateProfile.](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d70d6-107">List properties and relationships of the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d70d6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d70d6-108">Prerequisites</span></span>
<span data-ttu-id="d70d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d70d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d70d6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d70d6-111">Permission type</span></span>|<span data-ttu-id="d70d6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d70d6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d70d6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d70d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d70d6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d70d6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d70d6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d70d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d70d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d70d6-116">Not supported.</span></span>|
|<span data-ttu-id="d70d6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d70d6-117">Application</span></span>|<span data-ttu-id="d70d6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d70d6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d70d6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d70d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d70d6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d70d6-120">Request headers</span></span>
|<span data-ttu-id="d70d6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d70d6-121">Header</span></span>|<span data-ttu-id="d70d6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d70d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d70d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d70d6-123">Authorization</span></span>|<span data-ttu-id="d70d6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d70d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d70d6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d70d6-125">Accept</span></span>|<span data-ttu-id="d70d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d70d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d70d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d70d6-127">Request body</span></span>
<span data-ttu-id="d70d6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d70d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d70d6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d70d6-129">Response</span></span>
<span data-ttu-id="d70d6-130">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d70d6-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d70d6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d70d6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d70d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d70d6-132">Request</span></span>
<span data-ttu-id="d70d6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d70d6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d70d6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d70d6-134">Response</span></span>
<span data-ttu-id="d70d6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d70d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
      "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
      "renewalThresholdPercentage": 10,
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




