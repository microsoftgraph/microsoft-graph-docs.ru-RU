---
title: Список Виндовсупдатестатес
description: Список свойств и связей объектов Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7839ca7c75cf2c401bfc881c7504651d33f961e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735332"
---
# <a name="list-windowsupdatestates"></a><span data-ttu-id="16de2-103">Список Виндовсупдатестатес</span><span class="sxs-lookup"><span data-stu-id="16de2-103">List windowsUpdateStates</span></span>

<span data-ttu-id="16de2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16de2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16de2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16de2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16de2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16de2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16de2-107">Список свойств и связей объектов [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="16de2-107">List properties and relationships of the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16de2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16de2-108">Prerequisites</span></span>
<span data-ttu-id="16de2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16de2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16de2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16de2-111">Permission type</span></span>|<span data-ttu-id="16de2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16de2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16de2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16de2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="16de2-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="16de2-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="16de2-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16de2-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="16de2-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="16de2-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="16de2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16de2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="16de2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16de2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16de2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16de2-119">Not supported.</span></span>|
|<span data-ttu-id="16de2-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16de2-120">Application</span></span>||
| <span data-ttu-id="16de2-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="16de2-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="16de2-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16de2-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="16de2-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="16de2-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="16de2-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16de2-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16de2-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16de2-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="16de2-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16de2-126">Request headers</span></span>
|<span data-ttu-id="16de2-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16de2-127">Header</span></span>|<span data-ttu-id="16de2-128">Значение</span><span class="sxs-lookup"><span data-stu-id="16de2-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16de2-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16de2-129">Authorization</span></span>|<span data-ttu-id="16de2-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16de2-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16de2-131">Accept</span><span class="sxs-lookup"><span data-stu-id="16de2-131">Accept</span></span>|<span data-ttu-id="16de2-132">application/json</span><span class="sxs-lookup"><span data-stu-id="16de2-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16de2-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16de2-133">Request body</span></span>
<span data-ttu-id="16de2-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16de2-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16de2-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="16de2-135">Response</span></span>
<span data-ttu-id="16de2-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16de2-136">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16de2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="16de2-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="16de2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="16de2-138">Request</span></span>
<span data-ttu-id="16de2-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16de2-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

### <a name="response"></a><span data-ttu-id="16de2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="16de2-140">Response</span></span>
<span data-ttu-id="16de2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16de2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








