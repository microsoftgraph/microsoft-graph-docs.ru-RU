---
title: Список Импортедаппледевицеидентитиресултс
description: Список свойств и связей объектов Импортедаппледевицеидентитиресулт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2baf6c985f42169efe79ad6fcabd83bd4d92cbf3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813157"
---
# <a name="list-importedappledeviceidentityresults"></a><span data-ttu-id="3682e-103">Список Импортедаппледевицеидентитиресултс</span><span class="sxs-lookup"><span data-stu-id="3682e-103">List importedAppleDeviceIdentityResults</span></span>

> <span data-ttu-id="3682e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3682e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3682e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3682e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3682e-106">Список свойств и связей объектов [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="3682e-106">List properties and relationships of the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3682e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3682e-107">Prerequisites</span></span>
<span data-ttu-id="3682e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3682e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3682e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3682e-110">Permission type</span></span>|<span data-ttu-id="3682e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3682e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3682e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3682e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3682e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3682e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3682e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3682e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3682e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3682e-115">Not supported.</span></span>|
|<span data-ttu-id="3682e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3682e-116">Application</span></span>|<span data-ttu-id="3682e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3682e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3682e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3682e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="3682e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3682e-119">Request headers</span></span>
|<span data-ttu-id="3682e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3682e-120">Header</span></span>|<span data-ttu-id="3682e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3682e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3682e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3682e-122">Authorization</span></span>|<span data-ttu-id="3682e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3682e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3682e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3682e-124">Accept</span></span>|<span data-ttu-id="3682e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3682e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3682e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3682e-126">Request body</span></span>
<span data-ttu-id="3682e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3682e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3682e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3682e-128">Response</span></span>
<span data-ttu-id="3682e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3682e-129">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3682e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3682e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3682e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3682e-131">Request</span></span>
<span data-ttu-id="3682e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3682e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="3682e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3682e-133">Response</span></span>
<span data-ttu-id="3682e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3682e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 741

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
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
      "platform": "ios",
      "status": true
    }
  ]
}
```




