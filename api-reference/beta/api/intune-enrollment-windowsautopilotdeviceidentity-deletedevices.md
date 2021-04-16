---
title: deleteDevices action
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e026b15e67e64558d91774647ec460acebff7665
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864916"
---
# <a name="deletedevices-action"></a><span data-ttu-id="cb6ff-103">deleteDevices action</span><span class="sxs-lookup"><span data-stu-id="cb6ff-103">deleteDevices action</span></span>

<span data-ttu-id="cb6ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb6ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb6ff-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb6ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb6ff-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb6ff-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cb6ff-108">Prerequisites</span></span>
<span data-ttu-id="cb6ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb6ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb6ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb6ff-111">Permission type</span></span>|<span data-ttu-id="cb6ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb6ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb6ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb6ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb6ff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb6ff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cb6ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb6ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb6ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-116">Not supported.</span></span>|
|<span data-ttu-id="cb6ff-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="cb6ff-117">Application</span></span>|<span data-ttu-id="cb6ff-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb6ff-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb6ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb6ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/deleteDevices
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/deleteDevices
```

## <a name="request-headers"></a><span data-ttu-id="cb6ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb6ff-120">Request headers</span></span>
|<span data-ttu-id="cb6ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb6ff-121">Header</span></span>|<span data-ttu-id="cb6ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb6ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb6ff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb6ff-123">Authorization</span></span>|<span data-ttu-id="cb6ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb6ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb6ff-125">Accept</span></span>|<span data-ttu-id="cb6ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb6ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb6ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb6ff-127">Request body</span></span>
<span data-ttu-id="cb6ff-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cb6ff-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cb6ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb6ff-130">Property</span></span>|<span data-ttu-id="cb6ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb6ff-131">Type</span></span>|<span data-ttu-id="cb6ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb6ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb6ff-133">serialNumbers</span><span class="sxs-lookup"><span data-stu-id="cb6ff-133">serialNumbers</span></span>|<span data-ttu-id="cb6ff-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cb6ff-134">String collection</span></span>|<span data-ttu-id="cb6ff-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb6ff-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cb6ff-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb6ff-136">Response</span></span>
<span data-ttu-id="cb6ff-137">В случае успеха это действие возвращает код ответа и удаленную `200 OK` [коллекциюWindowsAutopilotDeviceState](../resources/intune-enrollment-deletedwindowsautopilotdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-137">If successful, this action returns a `200 OK` response code and a [deletedWindowsAutopilotDeviceState](../resources/intune-enrollment-deletedwindowsautopilotdevicestate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb6ff-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cb6ff-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb6ff-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb6ff-139">Request</span></span>
<span data-ttu-id="cb6ff-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/deleteDevices

Content-type: application/json
Content-length: 59

{
  "serialNumbers": [
    "Serial Numbers value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cb6ff-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb6ff-141">Response</span></span>
<span data-ttu-id="cb6ff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb6ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deletedWindowsAutopilotDeviceState",
      "serialNumber": "Serial Number value",
      "deviceRegistrationId": "Device Registration Id value",
      "deletionState": "failed",
      "errorMessage": "Error Message value"
    }
  ]
}
```




