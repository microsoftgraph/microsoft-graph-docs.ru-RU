---
title: Получение Виндовсупдатестате
description: Чтение свойств и связей объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c7cf4cb02d22f615cad9bd73eec337663bdf275
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537820"
---
# <a name="get-windowsupdatestate"></a><span data-ttu-id="5b510-103">Получение Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="5b510-103">Get windowsUpdateState</span></span>

> <span data-ttu-id="5b510-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b510-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b510-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b510-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b510-106">Чтение свойств и связей объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="5b510-106">Read properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b510-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b510-107">Prerequisites</span></span>
<span data-ttu-id="5b510-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b510-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b510-110">Permission type</span></span>|<span data-ttu-id="5b510-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b510-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b510-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b510-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5b510-113">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="5b510-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5b510-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b510-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5b510-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="5b510-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="5b510-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b510-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b510-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b510-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b510-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b510-118">Not supported.</span></span>|
|<span data-ttu-id="5b510-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b510-119">Application</span></span>||
| <span data-ttu-id="5b510-120">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="5b510-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5b510-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b510-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5b510-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="5b510-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="5b510-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b510-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b510-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b510-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b510-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b510-125">Optional query parameters</span></span>
<span data-ttu-id="5b510-126">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b510-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b510-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b510-127">Request headers</span></span>
|<span data-ttu-id="5b510-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b510-128">Header</span></span>|<span data-ttu-id="5b510-129">Значение</span><span class="sxs-lookup"><span data-stu-id="5b510-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b510-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b510-130">Authorization</span></span>|<span data-ttu-id="5b510-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b510-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b510-132">Accept</span><span class="sxs-lookup"><span data-stu-id="5b510-132">Accept</span></span>|<span data-ttu-id="5b510-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5b510-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b510-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b510-134">Request body</span></span>
<span data-ttu-id="5b510-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b510-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b510-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b510-136">Response</span></span>
<span data-ttu-id="5b510-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b510-137">If successful, this method returns a `200 OK` response code and [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b510-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5b510-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b510-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b510-139">Request</span></span>
<span data-ttu-id="5b510-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b510-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

### <a name="response"></a><span data-ttu-id="5b510-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b510-141">Response</span></span>
<span data-ttu-id="5b510-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b510-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






