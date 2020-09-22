---
title: Действие getTargetedUsersAndDevices
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69a8c8791a23f74b3b17efa48dc20a9870515ce4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095935"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="8b496-103">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="8b496-103">getTargetedUsersAndDevices action</span></span>

<span data-ttu-id="8b496-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b496-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b496-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b496-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b496-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b496-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b496-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8b496-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b496-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b496-108">Prerequisites</span></span>
<span data-ttu-id="8b496-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b496-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b496-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b496-111">Permission type</span></span>|<span data-ttu-id="8b496-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b496-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b496-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b496-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8b496-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8b496-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8b496-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b496-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8b496-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b496-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b496-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b496-117">Not supported.</span></span>|
|<span data-ttu-id="8b496-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b496-118">Application</span></span>||
| <span data-ttu-id="8b496-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8b496-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8b496-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b496-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b496-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b496-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="8b496-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b496-122">Request headers</span></span>
|<span data-ttu-id="8b496-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b496-123">Header</span></span>|<span data-ttu-id="8b496-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8b496-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b496-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b496-125">Authorization</span></span>|<span data-ttu-id="8b496-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b496-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b496-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8b496-127">Accept</span></span>|<span data-ttu-id="8b496-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8b496-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b496-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b496-129">Request body</span></span>
<span data-ttu-id="8b496-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b496-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8b496-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8b496-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8b496-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b496-132">Property</span></span>|<span data-ttu-id="8b496-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8b496-133">Type</span></span>|<span data-ttu-id="8b496-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8b496-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b496-135">девицеконфигуратионидс</span><span class="sxs-lookup"><span data-stu-id="8b496-135">deviceConfigurationIds</span></span>|<span data-ttu-id="8b496-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8b496-136">String collection</span></span>|<span data-ttu-id="8b496-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b496-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8b496-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b496-138">Response</span></span>
<span data-ttu-id="8b496-139">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [девицеконфигуратионтаржетедусеранддевице](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b496-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b496-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8b496-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b496-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b496-141">Request</span></span>
<span data-ttu-id="8b496-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b496-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/getTargetedUsersAndDevices

Content-type: application/json
Content-length: 78

{
  "deviceConfigurationIds": [
    "Device Configuration Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8b496-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b496-143">Response</span></span>
<span data-ttu-id="8b496-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b496-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
    }
  ]
}
```









