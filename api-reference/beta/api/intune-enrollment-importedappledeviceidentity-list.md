---
title: Список импортируемыхAppleDeviceIdentities
description: Список свойств и связей импортируемых объектовAppleDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe5fab753df0ae77d1bb05959861e7becf3bf8d9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142417"
---
# <a name="list-importedappledeviceidentities"></a><span data-ttu-id="8eb50-103">Список импортируемыхAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="8eb50-103">List importedAppleDeviceIdentities</span></span>

<span data-ttu-id="8eb50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eb50-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eb50-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8eb50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eb50-107">Список свойств и связей импортируемых [объектовAppleDeviceIdentity.](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="8eb50-107">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eb50-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8eb50-108">Prerequisites</span></span>
<span data-ttu-id="8eb50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb50-111">Permission type</span></span>|<span data-ttu-id="8eb50-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eb50-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eb50-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eb50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8eb50-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb50-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8eb50-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eb50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eb50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb50-116">Not supported.</span></span>|
|<span data-ttu-id="8eb50-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8eb50-117">Application</span></span>|<span data-ttu-id="8eb50-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb50-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eb50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eb50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="8eb50-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8eb50-120">Request headers</span></span>
|<span data-ttu-id="8eb50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8eb50-121">Header</span></span>|<span data-ttu-id="8eb50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8eb50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eb50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eb50-123">Authorization</span></span>|<span data-ttu-id="8eb50-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eb50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eb50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8eb50-125">Accept</span></span>|<span data-ttu-id="8eb50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8eb50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eb50-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8eb50-127">Request body</span></span>
<span data-ttu-id="8eb50-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8eb50-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8eb50-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eb50-129">Response</span></span>
<span data-ttu-id="8eb50-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb50-130">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb50-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8eb50-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eb50-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eb50-132">Request</span></span>
<span data-ttu-id="8eb50-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eb50-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="8eb50-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eb50-134">Response</span></span>
<span data-ttu-id="8eb50-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8eb50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": [
    {
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
  ]
}
```




