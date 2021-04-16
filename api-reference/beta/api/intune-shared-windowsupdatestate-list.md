---
title: Список windowsUpdateStates
description: Список свойств и связей объектов WindowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d9837763b952e9f2d980a61a4165a3232b1d5ab
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864720"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="02023-103">Список windowsUpdateStates</span><span class="sxs-lookup"><span data-stu-id="02023-103">List windowsUpdateStates</span></span>

<span data-ttu-id="02023-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02023-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02023-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02023-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02023-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02023-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02023-107">Список свойств и связей [объектов WindowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="02023-107">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02023-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02023-108">Prerequisites</span></span>
<span data-ttu-id="02023-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02023-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02023-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02023-111">Permission type</span></span>|<span data-ttu-id="02023-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02023-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02023-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02023-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="02023-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="02023-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="02023-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02023-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="02023-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="02023-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="02023-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02023-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="02023-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02023-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02023-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02023-119">Not supported.</span></span>|
|<span data-ttu-id="02023-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="02023-120">Application</span></span>||
| <span data-ttu-id="02023-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="02023-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="02023-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02023-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="02023-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="02023-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="02023-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02023-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02023-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02023-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="02023-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="02023-126">Request headers</span></span>
|<span data-ttu-id="02023-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02023-127">Header</span></span>|<span data-ttu-id="02023-128">Значение</span><span class="sxs-lookup"><span data-stu-id="02023-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02023-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02023-129">Authorization</span></span>|<span data-ttu-id="02023-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02023-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02023-131">Accept</span><span class="sxs-lookup"><span data-stu-id="02023-131">Accept</span></span>|<span data-ttu-id="02023-132">application/json</span><span class="sxs-lookup"><span data-stu-id="02023-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02023-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02023-133">Request body</span></span>
<span data-ttu-id="02023-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02023-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02023-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="02023-135">Response</span></span>
<span data-ttu-id="02023-136">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="02023-136">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02023-137">Пример</span><span class="sxs-lookup"><span data-stu-id="02023-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="02023-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="02023-138">Request</span></span>
<span data-ttu-id="02023-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02023-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="02023-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="02023-140">Response</span></span>
<span data-ttu-id="02023-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02023-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







