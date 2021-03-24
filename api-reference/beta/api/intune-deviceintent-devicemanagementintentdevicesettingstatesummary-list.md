---
title: Список deviceManagementIntentDeviceSettingStateSummaries
description: Список свойств и связей объектов deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd680143bd4d0effc6b66896f92eed096fce9d5b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132053"
---
# <a name="list-devicemanagementintentdevicesettingstatesummaries"></a><span data-ttu-id="f9ed3-103">Список deviceManagementIntentDeviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f9ed3-103">List deviceManagementIntentDeviceSettingStateSummaries</span></span>

<span data-ttu-id="f9ed3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9ed3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9ed3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9ed3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ed3-107">Список свойств и связей [объектов deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f9ed3-107">List properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9ed3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9ed3-108">Prerequisites</span></span>
<span data-ttu-id="f9ed3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ed3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ed3-111">Permission type</span></span>|<span data-ttu-id="f9ed3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9ed3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9ed3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9ed3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9ed3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ed3-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9ed3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9ed3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9ed3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-116">Not supported.</span></span>|
|<span data-ttu-id="f9ed3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f9ed3-117">Application</span></span>|<span data-ttu-id="f9ed3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ed3-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9ed3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9ed3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f9ed3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9ed3-120">Request headers</span></span>
|<span data-ttu-id="f9ed3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9ed3-121">Header</span></span>|<span data-ttu-id="f9ed3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9ed3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9ed3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9ed3-123">Authorization</span></span>|<span data-ttu-id="f9ed3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9ed3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9ed3-125">Accept</span></span>|<span data-ttu-id="f9ed3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9ed3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9ed3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9ed3-127">Request body</span></span>
<span data-ttu-id="f9ed3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ed3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ed3-129">Response</span></span>
<span data-ttu-id="f9ed3-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9ed3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f9ed3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9ed3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9ed3-132">Request</span></span>
<span data-ttu-id="f9ed3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="f9ed3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ed3-134">Response</span></span>
<span data-ttu-id="f9ed3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9ed3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
      "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
      "settingName": "Setting Name value",
      "compliantCount": 14,
      "conflictCount": 13,
      "errorCount": 10,
      "nonCompliantCount": 1,
      "notApplicableCount": 2,
      "remediatedCount": 15
    }
  ]
}
```




