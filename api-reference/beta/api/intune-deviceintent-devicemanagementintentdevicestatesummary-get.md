---
title: Получение Девицеманажементинтентдевицестатесуммари
description: Чтение свойств и связей объекта Девицеманажементинтентдевицестатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29e3b3bb50039eabb78efd43a65f5844eb5ee59e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087736"
---
# <a name="get-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="2cefd-103">Получение Девицеманажементинтентдевицестатесуммари</span><span class="sxs-lookup"><span data-stu-id="2cefd-103">Get deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="2cefd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cefd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cefd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cefd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cefd-106">Чтение свойств и связей объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="2cefd-106">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cefd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2cefd-107">Prerequisites</span></span>
<span data-ttu-id="2cefd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cefd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cefd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cefd-110">Permission type</span></span>|<span data-ttu-id="2cefd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cefd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cefd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cefd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2cefd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cefd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2cefd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cefd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cefd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cefd-115">Not supported.</span></span>|
|<span data-ttu-id="2cefd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cefd-116">Application</span></span>|<span data-ttu-id="2cefd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cefd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cefd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cefd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2cefd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2cefd-119">Optional query parameters</span></span>
<span data-ttu-id="2cefd-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2cefd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2cefd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cefd-121">Request headers</span></span>
|<span data-ttu-id="2cefd-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cefd-122">Header</span></span>|<span data-ttu-id="2cefd-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2cefd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cefd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cefd-124">Authorization</span></span>|<span data-ttu-id="2cefd-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cefd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cefd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2cefd-126">Accept</span></span>|<span data-ttu-id="2cefd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2cefd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cefd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cefd-128">Request body</span></span>
<span data-ttu-id="2cefd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cefd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cefd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2cefd-130">Response</span></span>
<span data-ttu-id="2cefd-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2cefd-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cefd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2cefd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cefd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cefd-133">Request</span></span>
<span data-ttu-id="2cefd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cefd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

### <a name="response"></a><span data-ttu-id="2cefd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cefd-135">Response</span></span>
<span data-ttu-id="2cefd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cefd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 321

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
    "id": "12230bf9-0bf9-1223-f90b-2312f90b2312",
    "conflictCount": 13,
    "errorCount": 10,
    "failedCount": 11,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12
  }
}
```






