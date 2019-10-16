---
title: Действие getTargetedUsersAndDevices
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3f12db1dc4d7023846c26e7824041470371dc26
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537052"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="3eef0-103">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="3eef0-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="3eef0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eef0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3eef0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3eef0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eef0-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3eef0-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eef0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3eef0-107">Prerequisites</span></span>
<span data-ttu-id="3eef0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eef0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eef0-110">Permission type</span></span>|<span data-ttu-id="3eef0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eef0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eef0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eef0-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3eef0-113">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="3eef0-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3eef0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eef0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3eef0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eef0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eef0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eef0-116">Not supported.</span></span>|
|<span data-ttu-id="3eef0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3eef0-117">Application</span></span>||
| <span data-ttu-id="3eef0-118">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="3eef0-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3eef0-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eef0-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eef0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eef0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="3eef0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3eef0-121">Request headers</span></span>
|<span data-ttu-id="3eef0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3eef0-122">Header</span></span>|<span data-ttu-id="3eef0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3eef0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eef0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3eef0-124">Authorization</span></span>|<span data-ttu-id="3eef0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eef0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eef0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3eef0-126">Accept</span></span>|<span data-ttu-id="3eef0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3eef0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eef0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eef0-128">Request body</span></span>
<span data-ttu-id="3eef0-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eef0-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3eef0-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3eef0-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3eef0-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eef0-131">Property</span></span>|<span data-ttu-id="3eef0-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3eef0-132">Type</span></span>|<span data-ttu-id="3eef0-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3eef0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eef0-134">девицеконфигуратионидс</span><span class="sxs-lookup"><span data-stu-id="3eef0-134">deviceConfigurationIds</span></span>|<span data-ttu-id="3eef0-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3eef0-135">String collection</span></span>|<span data-ttu-id="3eef0-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3eef0-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3eef0-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="3eef0-137">Response</span></span>
<span data-ttu-id="3eef0-138">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [девицеконфигуратионтаржетедусеранддевице](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3eef0-138">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eef0-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3eef0-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eef0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eef0-140">Request</span></span>
<span data-ttu-id="3eef0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eef0-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3eef0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eef0-142">Response</span></span>
<span data-ttu-id="3eef0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3eef0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






