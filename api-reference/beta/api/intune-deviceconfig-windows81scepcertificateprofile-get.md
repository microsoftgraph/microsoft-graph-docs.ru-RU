---
title: Получение windows81SCEPCertificateProfile
description: Чтение свойств и связей объекта windows81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ffcbd0860d0e5ef509d4528ea7f6044aecc8afd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143283"
---
# <a name="get-windows81scepcertificateprofile"></a><span data-ttu-id="d9e20-103">Получение windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d9e20-103">Get windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="d9e20-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e20-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9e20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e20-106">Чтение свойств и связей объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d9e20-106">Read properties and relationships of the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9e20-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9e20-107">Prerequisites</span></span>
<span data-ttu-id="d9e20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9e20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9e20-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9e20-110">Permission type</span></span>|<span data-ttu-id="d9e20-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9e20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9e20-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9e20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9e20-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9e20-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d9e20-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9e20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9e20-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e20-115">Not supported.</span></span>|
|<span data-ttu-id="d9e20-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9e20-116">Application</span></span>|<span data-ttu-id="d9e20-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9e20-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9e20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9e20-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d9e20-119">Optional query parameters</span></span>
<span data-ttu-id="d9e20-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d9e20-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9e20-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9e20-121">Request headers</span></span>
|<span data-ttu-id="d9e20-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9e20-122">Header</span></span>|<span data-ttu-id="d9e20-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d9e20-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9e20-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9e20-124">Authorization</span></span>|<span data-ttu-id="d9e20-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d9e20-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9e20-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d9e20-126">Accept</span></span>|<span data-ttu-id="d9e20-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d9e20-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9e20-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9e20-128">Request body</span></span>
<span data-ttu-id="d9e20-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9e20-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9e20-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9e20-130">Response</span></span>
<span data-ttu-id="d9e20-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9e20-131">If successful, this method returns a `200 OK` response code and [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9e20-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d9e20-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9e20-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9e20-133">Request</span></span>
<span data-ttu-id="d9e20-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9e20-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d9e20-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9e20-135">Response</span></span>
<span data-ttu-id="d9e20-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9e20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1522

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
    "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    ],
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectNameFormatString": "Subject Name Format String value",
    "keyUsage": "digitalSignature",
    "keySize": "size2048",
    "hashAlgorithm": "sha2",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
    "certificateStore": "machine"
  }
}
```




