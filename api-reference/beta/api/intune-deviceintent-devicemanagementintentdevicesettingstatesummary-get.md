---
title: Get deviceManagementIntentDeviceSettingStateSummary
description: Чтение свойств и связей объекта deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d1b14f0e15be0dbd941fa51b47c2262ceb686ce
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132074"
---
# <a name="get-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="9de16-103">Get deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="9de16-103">Get deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="9de16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9de16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9de16-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9de16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9de16-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9de16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9de16-107">Чтение свойств и связей [объекта deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9de16-107">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9de16-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9de16-108">Prerequisites</span></span>
<span data-ttu-id="9de16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9de16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9de16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9de16-111">Permission type</span></span>|<span data-ttu-id="9de16-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9de16-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9de16-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9de16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9de16-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de16-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9de16-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9de16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9de16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9de16-116">Not supported.</span></span>|
|<span data-ttu-id="9de16-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9de16-117">Application</span></span>|<span data-ttu-id="9de16-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de16-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9de16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9de16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9de16-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9de16-120">Optional query parameters</span></span>
<span data-ttu-id="9de16-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9de16-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9de16-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9de16-122">Request headers</span></span>
|<span data-ttu-id="9de16-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9de16-123">Header</span></span>|<span data-ttu-id="9de16-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9de16-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9de16-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9de16-125">Authorization</span></span>|<span data-ttu-id="9de16-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9de16-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9de16-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9de16-127">Accept</span></span>|<span data-ttu-id="9de16-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9de16-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9de16-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9de16-129">Request body</span></span>
<span data-ttu-id="9de16-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9de16-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9de16-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9de16-131">Response</span></span>
<span data-ttu-id="9de16-132">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9de16-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9de16-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9de16-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9de16-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9de16-134">Request</span></span>
<span data-ttu-id="9de16-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9de16-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="9de16-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9de16-136">Response</span></span>
<span data-ttu-id="9de16-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9de16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 366

{
  "value": {
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
}
```




