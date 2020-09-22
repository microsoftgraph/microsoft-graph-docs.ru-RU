---
title: Список Девицеманажементинтентдевицесеттингстатесуммариес
description: Список свойств и связей объектов Девицеманажементинтентдевицесеттингстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09d4c7f677eb294fec7f0de4d58793f17b8f4336
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050789"
---
# <a name="list-devicemanagementintentdevicesettingstatesummaries"></a><span data-ttu-id="a7149-103">Список Девицеманажементинтентдевицесеттингстатесуммариес</span><span class="sxs-lookup"><span data-stu-id="a7149-103">List deviceManagementIntentDeviceSettingStateSummaries</span></span>

<span data-ttu-id="a7149-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7149-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7149-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7149-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7149-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7149-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7149-107">Список свойств и связей объектов [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a7149-107">List properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7149-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7149-108">Prerequisites</span></span>
<span data-ttu-id="a7149-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7149-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7149-111">Permission type</span></span>|<span data-ttu-id="a7149-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7149-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7149-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7149-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7149-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7149-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a7149-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7149-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7149-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7149-116">Not supported.</span></span>|
|<span data-ttu-id="a7149-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7149-117">Application</span></span>|<span data-ttu-id="a7149-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7149-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7149-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7149-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a7149-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a7149-120">Request headers</span></span>
|<span data-ttu-id="a7149-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7149-121">Header</span></span>|<span data-ttu-id="a7149-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7149-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7149-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7149-123">Authorization</span></span>|<span data-ttu-id="a7149-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7149-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7149-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7149-125">Accept</span></span>|<span data-ttu-id="a7149-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7149-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7149-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7149-127">Request body</span></span>
<span data-ttu-id="a7149-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7149-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7149-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7149-129">Response</span></span>
<span data-ttu-id="a7149-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7149-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7149-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a7149-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7149-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7149-132">Request</span></span>
<span data-ttu-id="a7149-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7149-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="a7149-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7149-134">Response</span></span>
<span data-ttu-id="a7149-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7149-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






