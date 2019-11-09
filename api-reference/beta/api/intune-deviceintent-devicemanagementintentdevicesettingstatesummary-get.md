---
title: Получение Девицеманажементинтентдевицесеттингстатесуммари
description: Чтение свойств и связей объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 476e50e85f15fadc2a036bd20bb6cc6af523a502
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087750"
---
# <a name="get-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="1fea3-103">Получение Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="1fea3-103">Get deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="1fea3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fea3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fea3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fea3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fea3-106">Чтение свойств и связей объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1fea3-106">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fea3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1fea3-107">Prerequisites</span></span>
<span data-ttu-id="1fea3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fea3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fea3-110">Permission type</span></span>|<span data-ttu-id="1fea3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fea3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fea3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fea3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1fea3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fea3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1fea3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fea3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fea3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fea3-115">Not supported.</span></span>|
|<span data-ttu-id="1fea3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fea3-116">Application</span></span>|<span data-ttu-id="1fea3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fea3-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fea3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fea3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fea3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1fea3-119">Optional query parameters</span></span>
<span data-ttu-id="1fea3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1fea3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fea3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fea3-121">Request headers</span></span>
|<span data-ttu-id="1fea3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fea3-122">Header</span></span>|<span data-ttu-id="1fea3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1fea3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fea3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fea3-124">Authorization</span></span>|<span data-ttu-id="1fea3-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fea3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fea3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1fea3-126">Accept</span></span>|<span data-ttu-id="1fea3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1fea3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fea3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fea3-128">Request body</span></span>
<span data-ttu-id="1fea3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fea3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fea3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1fea3-130">Response</span></span>
<span data-ttu-id="1fea3-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fea3-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fea3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1fea3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fea3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fea3-133">Request</span></span>
<span data-ttu-id="1fea3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fea3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="1fea3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fea3-135">Response</span></span>
<span data-ttu-id="1fea3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fea3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






