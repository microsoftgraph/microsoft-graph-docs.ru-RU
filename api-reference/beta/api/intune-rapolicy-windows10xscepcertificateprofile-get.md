---
title: Получение windows10XSCEPCertificateProfile
description: Чтение свойств и связей объекта windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48c29d39c92694511237e805da2de9cef88fca9e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242427"
---
# <a name="get-windows10xscepcertificateprofile"></a><span data-ttu-id="39066-103">Получение windows10XSCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="39066-103">Get windows10XSCEPCertificateProfile</span></span>

<span data-ttu-id="39066-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39066-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39066-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39066-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39066-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39066-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39066-107">Чтение свойств и связей объекта [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="39066-107">Read properties and relationships of the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39066-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39066-108">Prerequisites</span></span>
<span data-ttu-id="39066-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39066-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39066-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39066-111">Permission type</span></span>|<span data-ttu-id="39066-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39066-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39066-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39066-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39066-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="39066-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="39066-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39066-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39066-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39066-116">Not supported.</span></span>|
|<span data-ttu-id="39066-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="39066-117">Application</span></span>|<span data-ttu-id="39066-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="39066-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39066-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39066-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39066-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39066-120">Optional query parameters</span></span>
<span data-ttu-id="39066-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="39066-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39066-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39066-122">Request headers</span></span>
|<span data-ttu-id="39066-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39066-123">Header</span></span>|<span data-ttu-id="39066-124">Значение</span><span class="sxs-lookup"><span data-stu-id="39066-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39066-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39066-125">Authorization</span></span>|<span data-ttu-id="39066-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39066-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39066-127">Accept</span><span class="sxs-lookup"><span data-stu-id="39066-127">Accept</span></span>|<span data-ttu-id="39066-128">application/json</span><span class="sxs-lookup"><span data-stu-id="39066-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39066-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39066-129">Request body</span></span>
<span data-ttu-id="39066-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39066-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39066-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="39066-131">Response</span></span>
<span data-ttu-id="39066-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39066-132">If successful, this method returns a `200 OK` response code and [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39066-133">Пример</span><span class="sxs-lookup"><span data-stu-id="39066-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="39066-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="39066-134">Request</span></span>
<span data-ttu-id="39066-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39066-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

### <a name="response"></a><span data-ttu-id="39066-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="39066-136">Response</span></span>
<span data-ttu-id="39066-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39066-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1388

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
    "id": "d174d58e-d58e-d174-8ed5-74d18ed574d1",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "certificateStore": "machine",
    "certificateValidityPeriodScale": "months",
    "certificateValidityPeriodValue": 14,
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "hashAlgorithm": [
      "sha2"
    ],
    "keySize": "size2048",
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "keyUsage": "digitalSignature",
    "renewalThresholdPercentage": 10,
    "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectAlternativeNameFormats": [
      {
        "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
        "sanType": "emailAddress",
        "name": "Name value"
      }
    ],
    "subjectNameFormatString": "Subject Name Format String value"
  }
}
```




