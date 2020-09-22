---
title: Список Усерекспериенцеаналитиксметричисториес
description: Список свойств и связей объектов Усерекспериенцеаналитиксметричистори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd1e9985e5de7cd706ef9d33e727f50ab022b921
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027799"
---
# <a name="list-userexperienceanalyticsmetrichistories"></a><span data-ttu-id="c5f94-103">Список Усерекспериенцеаналитиксметричисториес</span><span class="sxs-lookup"><span data-stu-id="c5f94-103">List userExperienceAnalyticsMetricHistories</span></span>

<span data-ttu-id="c5f94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5f94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5f94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f94-107">Список свойств и связей объектов [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f94-107">List properties and relationships of the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5f94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5f94-108">Prerequisites</span></span>
<span data-ttu-id="c5f94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5f94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5f94-111">Permission type</span></span>|<span data-ttu-id="c5f94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5f94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5f94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5f94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5f94-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5f94-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c5f94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5f94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5f94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5f94-116">Not supported.</span></span>|
|<span data-ttu-id="c5f94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5f94-117">Application</span></span>|<span data-ttu-id="c5f94-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5f94-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5f94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5f94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="c5f94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5f94-120">Request headers</span></span>
|<span data-ttu-id="c5f94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5f94-121">Header</span></span>|<span data-ttu-id="c5f94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5f94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5f94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5f94-123">Authorization</span></span>|<span data-ttu-id="c5f94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5f94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5f94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5f94-125">Accept</span></span>|<span data-ttu-id="c5f94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5f94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5f94-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5f94-127">Request body</span></span>
<span data-ttu-id="c5f94-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5f94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5f94-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5f94-129">Response</span></span>
<span data-ttu-id="c5f94-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5f94-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5f94-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c5f94-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5f94-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5f94-132">Request</span></span>
<span data-ttu-id="c5f94-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5f94-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
```

### <a name="response"></a><span data-ttu-id="c5f94-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5f94-134">Response</span></span>
<span data-ttu-id="c5f94-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5f94-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
      "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
      "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
    }
  ]
}
```






