---
title: Список Виндовсупдатестатес
description: Список свойств и связей объектов Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78b15612956f055cd3520b22de678cb5c44ed845
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201136"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="fa470-103">Список Виндовсупдатестатес</span><span class="sxs-lookup"><span data-stu-id="fa470-103">List windowsUpdateStates</span></span>

> <span data-ttu-id="fa470-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa470-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa470-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa470-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa470-106">Список свойств и связей объектов [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="fa470-106">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa470-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa470-107">Prerequisites</span></span>
<span data-ttu-id="fa470-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa470-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa470-110">Permission type</span></span>|<span data-ttu-id="fa470-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa470-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa470-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa470-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fa470-113">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="fa470-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fa470-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa470-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="fa470-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="fa470-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="fa470-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa470-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa470-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa470-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa470-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa470-118">Not supported.</span></span>|
|<span data-ttu-id="fa470-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa470-119">Application</span></span>||
| <span data-ttu-id="fa470-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="fa470-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fa470-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa470-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="fa470-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="fa470-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="fa470-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa470-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa470-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa470-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="fa470-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa470-125">Request headers</span></span>
|<span data-ttu-id="fa470-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa470-126">Header</span></span>|<span data-ttu-id="fa470-127">Значение</span><span class="sxs-lookup"><span data-stu-id="fa470-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa470-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa470-128">Authorization</span></span>|<span data-ttu-id="fa470-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa470-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa470-130">Accept</span><span class="sxs-lookup"><span data-stu-id="fa470-130">Accept</span></span>|<span data-ttu-id="fa470-131">application/json</span><span class="sxs-lookup"><span data-stu-id="fa470-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa470-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa470-132">Request body</span></span>
<span data-ttu-id="fa470-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa470-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa470-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa470-134">Response</span></span>
<span data-ttu-id="fa470-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa470-135">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa470-136">Пример</span><span class="sxs-lookup"><span data-stu-id="fa470-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa470-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa470-137">Request</span></span>
<span data-ttu-id="fa470-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa470-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="fa470-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa470-139">Response</span></span>
<span data-ttu-id="fa470-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa470-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 630

{
  "value": [
    {
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
  ]
}
```




