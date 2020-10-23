---
title: Список Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилсес
description: Список свойств и связей объектов Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d66f1e3bcba448d669d54684451aa0f1d043ebb8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735920"
---
# <a name="list-userexperienceanalyticsapphealthdeviceperformancedetailses"></a><span data-ttu-id="b0c96-103">Список Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилсес</span><span class="sxs-lookup"><span data-stu-id="b0c96-103">List userExperienceAnalyticsAppHealthDevicePerformanceDetailses</span></span>

<span data-ttu-id="b0c96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0c96-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0c96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0c96-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0c96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0c96-107">Список свойств и связей объектов [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c96-107">List properties and relationships of the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0c96-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b0c96-108">Prerequisites</span></span>
<span data-ttu-id="b0c96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0c96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0c96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0c96-111">Permission type</span></span>|<span data-ttu-id="b0c96-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0c96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0c96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0c96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0c96-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0c96-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b0c96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0c96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0c96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0c96-116">Not supported.</span></span>|
|<span data-ttu-id="b0c96-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0c96-117">Application</span></span>|<span data-ttu-id="b0c96-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0c96-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0c96-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0c96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a><span data-ttu-id="b0c96-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b0c96-120">Request headers</span></span>
|<span data-ttu-id="b0c96-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0c96-121">Header</span></span>|<span data-ttu-id="b0c96-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b0c96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0c96-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0c96-123">Authorization</span></span>|<span data-ttu-id="b0c96-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0c96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0c96-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0c96-125">Accept</span></span>|<span data-ttu-id="b0c96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0c96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0c96-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0c96-127">Request body</span></span>
<span data-ttu-id="b0c96-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0c96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0c96-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0c96-129">Response</span></span>
<span data-ttu-id="b0c96-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0c96-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0c96-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b0c96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0c96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0c96-132">Request</span></span>
<span data-ttu-id="b0c96-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0c96-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

### <a name="response"></a><span data-ttu-id="b0c96-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0c96-134">Response</span></span>
<span data-ttu-id="b0c96-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0c96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
      "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "eventType": "Event Type value",
      "appDisplayName": "App Display Name value",
      "deviceId": "Device Id value",
      "deviceDisplayName": "Device Display Name value"
    }
  ]
}
```





