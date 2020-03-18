---
title: Обновление windowsAutopilotSettings
description: Обновление свойств объекта windowsAutopilotSettings.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e81e2b83e6969f9752bb2f6170df9210ea869039
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804963"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="0db70-103">Обновление windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="0db70-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="0db70-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0db70-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0db70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0db70-106">Обновление свойств объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="0db70-106">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0db70-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0db70-107">Prerequisites</span></span>
<span data-ttu-id="0db70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0db70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0db70-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0db70-110">Permission type</span></span>|<span data-ttu-id="0db70-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0db70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0db70-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0db70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0db70-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db70-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0db70-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0db70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0db70-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db70-115">Not supported.</span></span>|
|<span data-ttu-id="0db70-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0db70-116">Application</span></span>|<span data-ttu-id="0db70-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db70-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0db70-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0db70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="0db70-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0db70-119">Request headers</span></span>
|<span data-ttu-id="0db70-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0db70-120">Header</span></span>|<span data-ttu-id="0db70-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0db70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0db70-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0db70-122">Authorization</span></span>|<span data-ttu-id="0db70-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0db70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0db70-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0db70-124">Accept</span></span>|<span data-ttu-id="0db70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0db70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0db70-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0db70-126">Request body</span></span>
<span data-ttu-id="0db70-127">В тексте запроса добавьте представление объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0db70-127">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="0db70-128">В следующей таблице приведены свойства, необходимые при создании [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="0db70-128">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="0db70-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0db70-129">Property</span></span>|<span data-ttu-id="0db70-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0db70-130">Type</span></span>|<span data-ttu-id="0db70-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0db70-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db70-132">id</span><span class="sxs-lookup"><span data-stu-id="0db70-132">id</span></span>|<span data-ttu-id="0db70-133">String</span><span class="sxs-lookup"><span data-stu-id="0db70-133">String</span></span>|<span data-ttu-id="0db70-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="0db70-134">The GUID for the object</span></span>|
|<span data-ttu-id="0db70-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0db70-135">lastSyncDateTime</span></span>|<span data-ttu-id="0db70-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db70-136">DateTimeOffset</span></span>|<span data-ttu-id="0db70-137">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="0db70-137">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="0db70-138">ластмануалсинктригжердатетиме</span><span class="sxs-lookup"><span data-stu-id="0db70-138">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="0db70-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db70-139">DateTimeOffset</span></span>|<span data-ttu-id="0db70-140">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="0db70-140">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="0db70-141">syncStatus</span><span class="sxs-lookup"><span data-stu-id="0db70-141">syncStatus</span></span>|[<span data-ttu-id="0db70-142">виндовсаутопилотсинкстатус</span><span class="sxs-lookup"><span data-stu-id="0db70-142">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="0db70-143">Указывает состояние синхронизации со службой синхронизации данных устройств (DDS).</span><span class="sxs-lookup"><span data-stu-id="0db70-143">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="0db70-144">Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0db70-144">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="0db70-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0db70-145">Response</span></span>
<span data-ttu-id="0db70-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0db70-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0db70-147">Пример</span><span class="sxs-lookup"><span data-stu-id="0db70-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="0db70-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="0db70-148">Request</span></span>
<span data-ttu-id="0db70-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0db70-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0db70-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0db70-150">Response</span></span>
<span data-ttu-id="0db70-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0db70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




