---
title: Список Импортедаппледевицеидентитиресултс
description: Список свойств и связей объектов Импортедаппледевицеидентитиресулт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37f06f2edd22281d3250d76b438fd89bfa3804f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233700"
---
# <a name="list-importedappledeviceidentityresults"></a><span data-ttu-id="c7470-103">Список Импортедаппледевицеидентитиресултс</span><span class="sxs-lookup"><span data-stu-id="c7470-103">List importedAppleDeviceIdentityResults</span></span>

<span data-ttu-id="c7470-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7470-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7470-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7470-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7470-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7470-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7470-107">Список свойств и связей объектов [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="c7470-107">List properties and relationships of the [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7470-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7470-108">Prerequisites</span></span>
<span data-ttu-id="c7470-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7470-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7470-111">Permission type</span></span>|<span data-ttu-id="c7470-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7470-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7470-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7470-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7470-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7470-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c7470-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7470-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7470-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7470-116">Not supported.</span></span>|
|<span data-ttu-id="c7470-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c7470-117">Application</span></span>|<span data-ttu-id="c7470-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7470-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7470-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7470-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="c7470-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c7470-120">Request headers</span></span>
|<span data-ttu-id="c7470-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7470-121">Header</span></span>|<span data-ttu-id="c7470-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7470-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7470-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7470-123">Authorization</span></span>|<span data-ttu-id="c7470-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7470-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7470-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7470-125">Accept</span></span>|<span data-ttu-id="c7470-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7470-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7470-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7470-127">Request body</span></span>
<span data-ttu-id="c7470-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7470-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7470-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7470-129">Response</span></span>
<span data-ttu-id="c7470-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7470-130">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7470-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c7470-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7470-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7470-132">Request</span></span>
<span data-ttu-id="c7470-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7470-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="c7470-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7470-134">Response</span></span>
<span data-ttu-id="c7470-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7470-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




