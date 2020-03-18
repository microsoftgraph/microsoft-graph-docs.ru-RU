---
title: Получение Виндовсупдатестате
description: Чтение свойств и связей объекта Виндовсупдатестате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa037ed30870e7d35b8f08a4909294b6ca57c791
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800433"
---
# <a name="get-windowsupdatestate"></a><span data-ttu-id="ea591-103">Получение Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="ea591-103">Get windowsUpdateState</span></span>

> <span data-ttu-id="ea591-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea591-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea591-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea591-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea591-106">Чтение свойств и связей объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ea591-106">Read properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea591-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea591-107">Prerequisites</span></span>
<span data-ttu-id="ea591-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea591-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea591-110">Permission type</span></span>|<span data-ttu-id="ea591-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea591-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea591-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea591-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ea591-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="ea591-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ea591-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea591-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ea591-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="ea591-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="ea591-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea591-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea591-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea591-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea591-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea591-118">Not supported.</span></span>|
|<span data-ttu-id="ea591-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea591-119">Application</span></span>||
| <span data-ttu-id="ea591-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="ea591-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ea591-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea591-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ea591-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="ea591-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="ea591-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea591-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea591-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea591-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea591-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea591-125">Optional query parameters</span></span>
<span data-ttu-id="ea591-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea591-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea591-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea591-127">Request headers</span></span>
|<span data-ttu-id="ea591-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea591-128">Header</span></span>|<span data-ttu-id="ea591-129">Значение</span><span class="sxs-lookup"><span data-stu-id="ea591-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea591-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea591-130">Authorization</span></span>|<span data-ttu-id="ea591-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea591-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea591-132">Accept</span><span class="sxs-lookup"><span data-stu-id="ea591-132">Accept</span></span>|<span data-ttu-id="ea591-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ea591-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea591-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea591-134">Request body</span></span>
<span data-ttu-id="ea591-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea591-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea591-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea591-136">Response</span></span>
<span data-ttu-id="ea591-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea591-137">If successful, this method returns a `200 OK` response code and [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea591-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ea591-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea591-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea591-139">Request</span></span>
<span data-ttu-id="ea591-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea591-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="ea591-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea591-141">Response</span></span>
<span data-ttu-id="ea591-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea591-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 594

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateState",
    "id": "3d92af00-af00-3d92-00af-923d00af923d",
    "deviceId": "Device Id value",
    "userId": "User Id value",
    "deviceDisplayName": "Device Display Name value",
    "userPrincipalName": "User Principal Name value",
    "status": "pendingInstallation",
    "qualityUpdateVersion": "Quality Update Version value",
    "featureUpdateVersion": "Feature Update Version value",
    "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```







