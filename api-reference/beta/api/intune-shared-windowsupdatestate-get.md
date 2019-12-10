---
title: Получение Виндовсупдатестате
description: Чтение свойств и связей объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da9c288a9dd678719bacfc6c9599f81d1cf509c2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939327"
---
# <a name="get-windowsupdatestate"></a><span data-ttu-id="eb7fa-103">Получение Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="eb7fa-103">Get windowsUpdateState</span></span>

> <span data-ttu-id="eb7fa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb7fa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb7fa-106">Чтение свойств и связей объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="eb7fa-106">Read properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb7fa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eb7fa-107">Prerequisites</span></span>
<span data-ttu-id="eb7fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb7fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb7fa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb7fa-110">Permission type</span></span>|<span data-ttu-id="eb7fa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb7fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb7fa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb7fa-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eb7fa-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="eb7fa-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="eb7fa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb7fa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="eb7fa-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="eb7fa-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="eb7fa-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb7fa-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eb7fa-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb7fa-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb7fa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-118">Not supported.</span></span>|
|<span data-ttu-id="eb7fa-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb7fa-119">Application</span></span>||
| <span data-ttu-id="eb7fa-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="eb7fa-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="eb7fa-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb7fa-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="eb7fa-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="eb7fa-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="eb7fa-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb7fa-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb7fa-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb7fa-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb7fa-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb7fa-125">Optional query parameters</span></span>
<span data-ttu-id="eb7fa-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb7fa-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb7fa-127">Request headers</span></span>
|<span data-ttu-id="eb7fa-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb7fa-128">Header</span></span>|<span data-ttu-id="eb7fa-129">Значение</span><span class="sxs-lookup"><span data-stu-id="eb7fa-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb7fa-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb7fa-130">Authorization</span></span>|<span data-ttu-id="eb7fa-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb7fa-132">Accept</span><span class="sxs-lookup"><span data-stu-id="eb7fa-132">Accept</span></span>|<span data-ttu-id="eb7fa-133">application/json</span><span class="sxs-lookup"><span data-stu-id="eb7fa-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb7fa-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb7fa-134">Request body</span></span>
<span data-ttu-id="eb7fa-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb7fa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb7fa-136">Response</span></span>
<span data-ttu-id="eb7fa-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-137">If successful, this method returns a `200 OK` response code and [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb7fa-138">Пример</span><span class="sxs-lookup"><span data-stu-id="eb7fa-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb7fa-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb7fa-139">Request</span></span>
<span data-ttu-id="eb7fa-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="eb7fa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb7fa-141">Response</span></span>
<span data-ttu-id="eb7fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb7fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








