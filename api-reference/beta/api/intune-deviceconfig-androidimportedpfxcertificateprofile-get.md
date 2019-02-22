---
title: Получение Андроидимпортедпфксцертификатепрофиле
description: Чтение свойств и связей объекта Андроидимпортедпфксцертификатепрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27f0bc60c082e5d3905346730b17aa64479b6763
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165158"
---
# <a name="get-androidimportedpfxcertificateprofile"></a><span data-ttu-id="72029-103">Получение Андроидимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="72029-103">Get androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="72029-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72029-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72029-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72029-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72029-106">Чтение свойств и связей объекта [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="72029-106">Read properties and relationships of the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72029-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72029-107">Prerequisites</span></span>
<span data-ttu-id="72029-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="72029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="72029-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72029-110">Permission type</span></span>|<span data-ttu-id="72029-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72029-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72029-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72029-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72029-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="72029-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="72029-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72029-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72029-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72029-115">Not supported.</span></span>|
|<span data-ttu-id="72029-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72029-116">Application</span></span>|<span data-ttu-id="72029-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72029-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72029-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72029-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72029-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72029-119">Optional query parameters</span></span>
<span data-ttu-id="72029-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72029-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72029-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72029-121">Request headers</span></span>
|<span data-ttu-id="72029-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72029-122">Header</span></span>|<span data-ttu-id="72029-123">Значение</span><span class="sxs-lookup"><span data-stu-id="72029-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72029-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72029-124">Authorization</span></span>|<span data-ttu-id="72029-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="72029-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72029-126">Accept</span><span class="sxs-lookup"><span data-stu-id="72029-126">Accept</span></span>|<span data-ttu-id="72029-127">application/json</span><span class="sxs-lookup"><span data-stu-id="72029-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72029-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72029-128">Request body</span></span>
<span data-ttu-id="72029-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72029-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72029-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="72029-130">Response</span></span>
<span data-ttu-id="72029-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72029-131">If successful, this method returns a `200 OK` response code and [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72029-132">Пример</span><span class="sxs-lookup"><span data-stu-id="72029-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="72029-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="72029-133">Request</span></span>
<span data-ttu-id="72029-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72029-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="72029-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="72029-135">Response</span></span>
<span data-ttu-id="72029-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": {
    "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
    "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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




