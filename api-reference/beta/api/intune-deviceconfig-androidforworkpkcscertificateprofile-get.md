---
title: Получение androidForWorkPkcsCertificateProfile
description: Чтение свойств и связей объекта androidForWorkPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0245ecf1a4fbc08a6b1b6def4ccc56fc849a159e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084848"
---
# <a name="get-androidforworkpkcscertificateprofile"></a><span data-ttu-id="21bde-103">Получение androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="21bde-103">Get androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="21bde-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bde-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21bde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bde-106">Чтение свойств и связей объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="21bde-106">Read properties and relationships of the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21bde-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21bde-107">Prerequisites</span></span>
<span data-ttu-id="21bde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21bde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21bde-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21bde-110">Permission type</span></span>|<span data-ttu-id="21bde-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21bde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21bde-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21bde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21bde-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21bde-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21bde-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21bde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21bde-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bde-115">Not supported.</span></span>|
|<span data-ttu-id="21bde-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21bde-116">Application</span></span>|<span data-ttu-id="21bde-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21bde-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21bde-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21bde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21bde-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="21bde-119">Optional query parameters</span></span>
<span data-ttu-id="21bde-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="21bde-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21bde-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21bde-121">Request headers</span></span>
|<span data-ttu-id="21bde-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21bde-122">Header</span></span>|<span data-ttu-id="21bde-123">Значение</span><span class="sxs-lookup"><span data-stu-id="21bde-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21bde-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21bde-124">Authorization</span></span>|<span data-ttu-id="21bde-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21bde-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21bde-126">Accept</span><span class="sxs-lookup"><span data-stu-id="21bde-126">Accept</span></span>|<span data-ttu-id="21bde-127">application/json</span><span class="sxs-lookup"><span data-stu-id="21bde-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21bde-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21bde-128">Request body</span></span>
<span data-ttu-id="21bde-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21bde-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21bde-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="21bde-130">Response</span></span>
<span data-ttu-id="21bde-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21bde-131">If successful, this method returns a `200 OK` response code and [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21bde-132">Пример</span><span class="sxs-lookup"><span data-stu-id="21bde-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="21bde-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="21bde-133">Request</span></span>
<span data-ttu-id="21bde-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21bde-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="21bde-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="21bde-135">Response</span></span>
<span data-ttu-id="21bde-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21bde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2025

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
    "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
    "subjectNameFormat": "commonNameIncludingEmail",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "subjectAlternativeNameType": "emailAddress",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
  }
}
```






