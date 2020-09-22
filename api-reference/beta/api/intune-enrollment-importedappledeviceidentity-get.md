---
title: Получение Импортедаппледевицеидентити
description: Чтение свойств и связей объекта Импортедаппледевицеидентити.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80730a26a31bbbedc7f44c0853ac5886a194e551
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986576"
---
# <a name="get-importedappledeviceidentity"></a><span data-ttu-id="5ef88-103">Получение Импортедаппледевицеидентити</span><span class="sxs-lookup"><span data-stu-id="5ef88-103">Get importedAppleDeviceIdentity</span></span>

<span data-ttu-id="5ef88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ef88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ef88-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ef88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ef88-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ef88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ef88-107">Чтение свойств и связей объекта [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5ef88-107">Read properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ef88-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ef88-108">Prerequisites</span></span>
<span data-ttu-id="5ef88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ef88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ef88-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ef88-111">Permission type</span></span>|<span data-ttu-id="5ef88-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ef88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ef88-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ef88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ef88-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ef88-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5ef88-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ef88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ef88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ef88-116">Not supported.</span></span>|
|<span data-ttu-id="5ef88-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ef88-117">Application</span></span>|<span data-ttu-id="5ef88-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ef88-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ef88-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ef88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ef88-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5ef88-120">Optional query parameters</span></span>
<span data-ttu-id="5ef88-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ef88-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ef88-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ef88-122">Request headers</span></span>
|<span data-ttu-id="5ef88-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ef88-123">Header</span></span>|<span data-ttu-id="5ef88-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5ef88-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ef88-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ef88-125">Authorization</span></span>|<span data-ttu-id="5ef88-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ef88-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ef88-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5ef88-127">Accept</span></span>|<span data-ttu-id="5ef88-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5ef88-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ef88-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ef88-129">Request body</span></span>
<span data-ttu-id="5ef88-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ef88-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ef88-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ef88-131">Response</span></span>
<span data-ttu-id="5ef88-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ef88-132">If successful, this method returns a `200 OK` response code and [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ef88-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5ef88-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ef88-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ef88-134">Request</span></span>
<span data-ttu-id="5ef88-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ef88-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="5ef88-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ef88-136">Response</span></span>
<span data-ttu-id="5ef88-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ef88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 672

{
  "value": {
    "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
    "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
    "serialNumber": "Serial Number value",
    "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
    "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
    "isSupervised": true,
    "discoverySource": "adminImport",
    "isDeleted": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
    "description": "Description value",
    "enrollmentState": "enrolled",
    "platform": "ios"
  }
}
```






