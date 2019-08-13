---
title: Список windows81CertificateProfileBases
description: Список свойств и связей объектов windows81CertificateProfileBase.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da00031f7ccaa7cf69ca80ad5566e9a83e165bec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314247"
---
# <a name="list-windows81certificateprofilebases"></a><span data-ttu-id="a1703-103">Список windows81CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="a1703-103">List windows81CertificateProfileBases</span></span>

> <span data-ttu-id="a1703-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1703-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1703-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1703-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1703-106">Список свойств и связей объектов [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="a1703-106">List properties and relationships of the [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1703-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1703-107">Prerequisites</span></span>
<span data-ttu-id="a1703-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1703-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1703-110">Permission type</span></span>|<span data-ttu-id="a1703-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1703-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1703-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1703-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1703-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1703-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1703-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1703-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1703-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1703-115">Not supported.</span></span>|
|<span data-ttu-id="a1703-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1703-116">Application</span></span>|<span data-ttu-id="a1703-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1703-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1703-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1703-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a1703-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1703-119">Request headers</span></span>
|<span data-ttu-id="a1703-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1703-120">Header</span></span>|<span data-ttu-id="a1703-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1703-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1703-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1703-122">Authorization</span></span>|<span data-ttu-id="a1703-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1703-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1703-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1703-124">Accept</span></span>|<span data-ttu-id="a1703-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1703-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1703-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1703-126">Request body</span></span>
<span data-ttu-id="a1703-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1703-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1703-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1703-128">Response</span></span>
<span data-ttu-id="a1703-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1703-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1703-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a1703-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1703-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1703-131">Request</span></span>
<span data-ttu-id="a1703-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1703-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a1703-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1703-133">Response</span></span>
<span data-ttu-id="a1703-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1703-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2100

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CertificateProfileBase",
      "id": "61cae8b8-e8b8-61ca-b8e8-ca61b8e8ca61",
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
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ]
    }
  ]
}
```






