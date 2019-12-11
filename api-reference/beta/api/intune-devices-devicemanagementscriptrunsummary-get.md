---
title: Получение Девицеманажементскриптрунсуммари
description: Чтение свойств и связей объекта Девицеманажементскриптрунсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6d003f037cf7aa123c4d432ea2dd914c1bfea30
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944927"
---
# <a name="get-devicemanagementscriptrunsummary"></a><span data-ttu-id="a1dca-103">Получение Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="a1dca-103">Get deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="a1dca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1dca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1dca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1dca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1dca-106">Чтение свойств и связей объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="a1dca-106">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1dca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1dca-107">Prerequisites</span></span>
<span data-ttu-id="a1dca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1dca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1dca-110">Permission type</span></span>|<span data-ttu-id="a1dca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1dca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1dca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1dca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1dca-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1dca-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a1dca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1dca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1dca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1dca-115">Not supported.</span></span>|
|<span data-ttu-id="a1dca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1dca-116">Application</span></span>|<span data-ttu-id="a1dca-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1dca-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1dca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1dca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1dca-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1dca-119">Optional query parameters</span></span>
<span data-ttu-id="a1dca-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1dca-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1dca-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1dca-121">Request headers</span></span>
|<span data-ttu-id="a1dca-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1dca-122">Header</span></span>|<span data-ttu-id="a1dca-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a1dca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1dca-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1dca-124">Authorization</span></span>|<span data-ttu-id="a1dca-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1dca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1dca-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a1dca-126">Accept</span></span>|<span data-ttu-id="a1dca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1dca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1dca-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1dca-128">Request body</span></span>
<span data-ttu-id="a1dca-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1dca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1dca-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1dca-130">Response</span></span>
<span data-ttu-id="a1dca-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1dca-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1dca-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a1dca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1dca-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1dca-133">Request</span></span>
<span data-ttu-id="a1dca-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1dca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
```

### <a name="response"></a><span data-ttu-id="a1dca-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1dca-135">Response</span></span>
<span data-ttu-id="a1dca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1dca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
    "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
    "successDeviceCount": 2,
    "errorDeviceCount": 0,
    "successUserCount": 0,
    "errorUserCount": 14
  }
}
```





