---
title: Действие getTargetedUsersAndDevices
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a7aee503cacd2e4aa9f45b53dc46a2494f61827
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702987"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="16511-103">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="16511-103">getTargetedUsersAndDevices action</span></span>

<span data-ttu-id="16511-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16511-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16511-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16511-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16511-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16511-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16511-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="16511-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16511-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16511-108">Prerequisites</span></span>
<span data-ttu-id="16511-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16511-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16511-111">Permission type</span></span>|<span data-ttu-id="16511-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16511-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16511-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16511-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="16511-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="16511-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="16511-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16511-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="16511-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16511-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16511-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16511-117">Not supported.</span></span>|
|<span data-ttu-id="16511-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16511-118">Application</span></span>||
| <span data-ttu-id="16511-119">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="16511-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="16511-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16511-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16511-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16511-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="16511-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16511-122">Request headers</span></span>
|<span data-ttu-id="16511-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16511-123">Header</span></span>|<span data-ttu-id="16511-124">Значение</span><span class="sxs-lookup"><span data-stu-id="16511-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16511-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16511-125">Authorization</span></span>|<span data-ttu-id="16511-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16511-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16511-127">Accept</span><span class="sxs-lookup"><span data-stu-id="16511-127">Accept</span></span>|<span data-ttu-id="16511-128">application/json</span><span class="sxs-lookup"><span data-stu-id="16511-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16511-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16511-129">Request body</span></span>
<span data-ttu-id="16511-130">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16511-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="16511-131">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="16511-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="16511-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="16511-132">Property</span></span>|<span data-ttu-id="16511-133">Тип</span><span class="sxs-lookup"><span data-stu-id="16511-133">Type</span></span>|<span data-ttu-id="16511-134">Описание</span><span class="sxs-lookup"><span data-stu-id="16511-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16511-135">девицеконфигуратионидс</span><span class="sxs-lookup"><span data-stu-id="16511-135">deviceConfigurationIds</span></span>|<span data-ttu-id="16511-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="16511-136">String collection</span></span>|<span data-ttu-id="16511-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="16511-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="16511-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="16511-138">Response</span></span>
<span data-ttu-id="16511-139">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [девицеконфигуратионтаржетедусеранддевице](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16511-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16511-140">Пример</span><span class="sxs-lookup"><span data-stu-id="16511-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="16511-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="16511-141">Request</span></span>
<span data-ttu-id="16511-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16511-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16511-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="16511-143">Response</span></span>
<span data-ttu-id="16511-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16511-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








