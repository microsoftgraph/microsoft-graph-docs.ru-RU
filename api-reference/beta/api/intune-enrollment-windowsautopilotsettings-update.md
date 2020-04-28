---
title: Обновление windowsAutopilotSettings
description: Обновление свойств объекта windowsAutopilotSettings.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29ec5af7b5b900bcd6ec8f976c665782d371c165
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452284"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="2c624-103">Обновление windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="2c624-103">Update windowsAutopilotSettings</span></span>

<span data-ttu-id="2c624-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c624-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c624-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c624-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c624-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c624-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c624-107">Обновление свойств объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="2c624-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c624-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2c624-108">Prerequisites</span></span>
<span data-ttu-id="2c624-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c624-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c624-111">Permission type</span></span>|<span data-ttu-id="2c624-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c624-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c624-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c624-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c624-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c624-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2c624-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c624-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c624-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c624-116">Not supported.</span></span>|
|<span data-ttu-id="2c624-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c624-117">Application</span></span>|<span data-ttu-id="2c624-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c624-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c624-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c624-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="2c624-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2c624-120">Request headers</span></span>
|<span data-ttu-id="2c624-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c624-121">Header</span></span>|<span data-ttu-id="2c624-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2c624-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c624-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c624-123">Authorization</span></span>|<span data-ttu-id="2c624-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c624-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c624-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2c624-125">Accept</span></span>|<span data-ttu-id="2c624-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c624-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c624-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c624-127">Request body</span></span>
<span data-ttu-id="2c624-128">В тексте запроса добавьте представление объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c624-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="2c624-129">В следующей таблице приведены свойства, необходимые при создании [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="2c624-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="2c624-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c624-130">Property</span></span>|<span data-ttu-id="2c624-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2c624-131">Type</span></span>|<span data-ttu-id="2c624-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2c624-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c624-133">id</span><span class="sxs-lookup"><span data-stu-id="2c624-133">id</span></span>|<span data-ttu-id="2c624-134">String</span><span class="sxs-lookup"><span data-stu-id="2c624-134">String</span></span>|<span data-ttu-id="2c624-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="2c624-135">The GUID for the object</span></span>|
|<span data-ttu-id="2c624-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2c624-136">lastSyncDateTime</span></span>|<span data-ttu-id="2c624-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c624-137">DateTimeOffset</span></span>|<span data-ttu-id="2c624-138">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="2c624-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="2c624-139">ластмануалсинктригжердатетиме</span><span class="sxs-lookup"><span data-stu-id="2c624-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="2c624-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c624-140">DateTimeOffset</span></span>|<span data-ttu-id="2c624-141">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="2c624-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="2c624-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="2c624-142">syncStatus</span></span>|[<span data-ttu-id="2c624-143">виндовсаутопилотсинкстатус</span><span class="sxs-lookup"><span data-stu-id="2c624-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="2c624-144">Указывает состояние синхронизации со службой синхронизации данных устройств (DDS).</span><span class="sxs-lookup"><span data-stu-id="2c624-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="2c624-145">Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2c624-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="2c624-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c624-146">Response</span></span>
<span data-ttu-id="2c624-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c624-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c624-148">Пример</span><span class="sxs-lookup"><span data-stu-id="2c624-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c624-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c624-149">Request</span></span>
<span data-ttu-id="2c624-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c624-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="2c624-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c624-151">Response</span></span>
<span data-ttu-id="2c624-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c624-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```



