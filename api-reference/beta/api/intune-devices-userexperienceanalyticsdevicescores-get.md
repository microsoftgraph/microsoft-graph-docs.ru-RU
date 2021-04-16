---
title: Get userExperienceAnalyticsDeviceScores
description: Чтение свойств и связей объекта userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11114c40aa29de5c78283d065c30355a46fbea1f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869062"
---
# <a name="get-userexperienceanalyticsdevicescores"></a><span data-ttu-id="f3fb7-103">Get userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="f3fb7-103">Get userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="f3fb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3fb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3fb7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3fb7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3fb7-107">Чтение свойств и связей [объекта userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="f3fb7-107">Read properties and relationships of the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3fb7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3fb7-108">Prerequisites</span></span>
<span data-ttu-id="f3fb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3fb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3fb7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3fb7-111">Permission type</span></span>|<span data-ttu-id="f3fb7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3fb7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3fb7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3fb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3fb7-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fb7-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3fb7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3fb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3fb7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-116">Not supported.</span></span>|
|<span data-ttu-id="f3fb7-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f3fb7-117">Application</span></span>|<span data-ttu-id="f3fb7-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3fb7-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3fb7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3fb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3fb7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3fb7-120">Optional query parameters</span></span>
<span data-ttu-id="f3fb7-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3fb7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3fb7-122">Request headers</span></span>
|<span data-ttu-id="f3fb7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3fb7-123">Header</span></span>|<span data-ttu-id="f3fb7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f3fb7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3fb7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3fb7-125">Authorization</span></span>|<span data-ttu-id="f3fb7-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3fb7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f3fb7-127">Accept</span></span>|<span data-ttu-id="f3fb7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f3fb7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3fb7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3fb7-129">Request body</span></span>
<span data-ttu-id="f3fb7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3fb7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3fb7-131">Response</span></span>
<span data-ttu-id="f3fb7-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3fb7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f3fb7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3fb7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3fb7-134">Request</span></span>
<span data-ttu-id="f3fb7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

### <a name="response"></a><span data-ttu-id="f3fb7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3fb7-136">Response</span></span>
<span data-ttu-id="f3fb7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3fb7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
    "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
    "deviceName": "Device Name value",
    "model": "Model value",
    "manufacturer": "Manufacturer value",
    "endpointAnalyticsScore": 7.333333333333333,
    "startupPerformanceScore": 7.666666666666667,
    "appReliabilityScore": 6.333333333333333
  }
}
```




