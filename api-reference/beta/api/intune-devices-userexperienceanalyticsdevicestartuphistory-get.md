---
title: Get userExperienceAnalyticsDeviceStartupHistory
description: Чтение свойств и связей объекта userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d8fd2dffe82953207d889af51131bded3f30c4e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154149"
---
# <a name="get-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="1eba3-103">Get userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="1eba3-103">Get userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="1eba3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eba3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1eba3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1eba3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eba3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1eba3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eba3-107">Чтение свойств и связей [объекта userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)</span><span class="sxs-lookup"><span data-stu-id="1eba3-107">Read properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1eba3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1eba3-108">Prerequisites</span></span>
<span data-ttu-id="1eba3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eba3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1eba3-111">Permission type</span></span>|<span data-ttu-id="1eba3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1eba3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1eba3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1eba3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1eba3-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eba3-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1eba3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1eba3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1eba3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1eba3-116">Not supported.</span></span>|
|<span data-ttu-id="1eba3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1eba3-117">Application</span></span>|<span data-ttu-id="1eba3-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eba3-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1eba3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1eba3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1eba3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1eba3-120">Optional query parameters</span></span>
<span data-ttu-id="1eba3-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1eba3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1eba3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1eba3-122">Request headers</span></span>
|<span data-ttu-id="1eba3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1eba3-123">Header</span></span>|<span data-ttu-id="1eba3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1eba3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1eba3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1eba3-125">Authorization</span></span>|<span data-ttu-id="1eba3-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1eba3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1eba3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1eba3-127">Accept</span></span>|<span data-ttu-id="1eba3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1eba3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eba3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1eba3-129">Request body</span></span>
<span data-ttu-id="1eba3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1eba3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1eba3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1eba3-131">Response</span></span>
<span data-ttu-id="1eba3-132">В случае успеха этот метод возвращает код ответа и `200 OK` [объект userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1eba3-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eba3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1eba3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1eba3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1eba3-134">Request</span></span>
<span data-ttu-id="1eba3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1eba3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

### <a name="response"></a><span data-ttu-id="1eba3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1eba3-136">Response</span></span>
<span data-ttu-id="1eba3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1eba3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
    "id": "13357123-7123-1335-2371-351323713513",
    "deviceId": "Device Id value",
    "startTime": "2017-01-01T00:03:29.2730865-08:00",
    "coreBootTimeInMs": 0,
    "groupPolicyBootTimeInMs": 7,
    "featureUpdateBootTimeInMs": 9,
    "totalBootTimeInMs": 1,
    "groupPolicyLoginTimeInMs": 8,
    "coreLoginTimeInMs": 1,
    "responsiveDesktopTimeInMs": 9,
    "totalLoginTimeInMs": 2,
    "isFirstLogin": true,
    "isFeatureUpdate": true,
    "operatingSystemVersion": "Operating System Version value",
    "restartCategory": "restartWithUpdate",
    "restartStopCode": "Restart Stop Code value",
    "restartFaultBucket": "Restart Fault Bucket value"
  }
}
```




