---
title: Получение Андроидфорворкимпортедпфксцертификатепрофиле
description: Чтение свойств и связей объекта Андроидфорворкимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7475864f90584323731b5ab1f02144e178400106
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37169400"
---
# <a name="get-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="9b4ac-103">Получение Андроидфорворкимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="9b4ac-103">Get androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="9b4ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b4ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b4ac-106">Чтение свойств и связей объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9b4ac-106">Read properties and relationships of the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b4ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b4ac-107">Prerequisites</span></span>
<span data-ttu-id="9b4ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b4ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b4ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b4ac-110">Permission type</span></span>|<span data-ttu-id="9b4ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b4ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b4ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b4ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b4ac-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b4ac-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b4ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b4ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b4ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-115">Not supported.</span></span>|
|<span data-ttu-id="9b4ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b4ac-116">Application</span></span>|<span data-ttu-id="9b4ac-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b4ac-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b4ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b4ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b4ac-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9b4ac-119">Optional query parameters</span></span>
<span data-ttu-id="9b4ac-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b4ac-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b4ac-121">Request headers</span></span>
|<span data-ttu-id="9b4ac-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b4ac-122">Header</span></span>|<span data-ttu-id="9b4ac-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9b4ac-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b4ac-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b4ac-124">Authorization</span></span>|<span data-ttu-id="9b4ac-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b4ac-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9b4ac-126">Accept</span></span>|<span data-ttu-id="9b4ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9b4ac-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b4ac-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b4ac-128">Request body</span></span>
<span data-ttu-id="9b4ac-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b4ac-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b4ac-130">Response</span></span>
<span data-ttu-id="9b4ac-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-131">If successful, this method returns a `200 OK` response code and [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b4ac-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9b4ac-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b4ac-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b4ac-133">Request</span></span>
<span data-ttu-id="9b4ac-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9b4ac-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b4ac-135">Response</span></span>
<span data-ttu-id="9b4ac-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b4ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1780

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
    "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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
    "intendedPurpose": "smimeEncryption"
  }
}
```




