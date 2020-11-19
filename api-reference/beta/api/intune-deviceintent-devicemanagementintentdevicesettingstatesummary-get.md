---
title: Получение Девицеманажементинтентдевицесеттингстатесуммари
description: Чтение свойств и связей объекта Девицеманажементинтентдевицесеттингстатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec9b75b0b09276f457b62f600906c06363770c3c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49278109"
---
# <a name="get-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="a22fc-103">Получение Девицеманажементинтентдевицесеттингстатесуммари</span><span class="sxs-lookup"><span data-stu-id="a22fc-103">Get deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="a22fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a22fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a22fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a22fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a22fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a22fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a22fc-107">Чтение свойств и связей объекта [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a22fc-107">Read properties and relationships of the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a22fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a22fc-108">Prerequisites</span></span>
<span data-ttu-id="a22fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a22fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a22fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a22fc-111">Permission type</span></span>|<span data-ttu-id="a22fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a22fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a22fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a22fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a22fc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a22fc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a22fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a22fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a22fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a22fc-116">Not supported.</span></span>|
|<span data-ttu-id="a22fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a22fc-117">Application</span></span>|<span data-ttu-id="a22fc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a22fc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a22fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a22fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a22fc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a22fc-120">Optional query parameters</span></span>
<span data-ttu-id="a22fc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a22fc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a22fc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a22fc-122">Request headers</span></span>
|<span data-ttu-id="a22fc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a22fc-123">Header</span></span>|<span data-ttu-id="a22fc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a22fc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a22fc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a22fc-125">Authorization</span></span>|<span data-ttu-id="a22fc-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a22fc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a22fc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a22fc-127">Accept</span></span>|<span data-ttu-id="a22fc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a22fc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a22fc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a22fc-129">Request body</span></span>
<span data-ttu-id="a22fc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a22fc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a22fc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a22fc-131">Response</span></span>
<span data-ttu-id="a22fc-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтентдевицесеттингстатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a22fc-132">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a22fc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a22fc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a22fc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a22fc-134">Request</span></span>
<span data-ttu-id="a22fc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a22fc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="a22fc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a22fc-136">Response</span></span>
<span data-ttu-id="a22fc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a22fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




