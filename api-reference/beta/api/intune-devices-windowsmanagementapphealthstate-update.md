---
title: Обновление Виндовсманажементапфеалсстате
description: Обновление свойств объекта Виндовсманажементапфеалсстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7724051789f00d1cc1c8a0ccb625f838e6e2eee7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972184"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="1481d-103">Обновление Виндовсманажементапфеалсстате</span><span class="sxs-lookup"><span data-stu-id="1481d-103">Update windowsManagementAppHealthState</span></span>

<span data-ttu-id="1481d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1481d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1481d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1481d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1481d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1481d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1481d-107">Обновление свойств объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="1481d-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1481d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1481d-108">Prerequisites</span></span>
<span data-ttu-id="1481d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1481d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1481d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1481d-111">Permission type</span></span>|<span data-ttu-id="1481d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1481d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1481d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1481d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1481d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1481d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1481d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1481d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1481d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1481d-116">Not supported.</span></span>|
|<span data-ttu-id="1481d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1481d-117">Application</span></span>|<span data-ttu-id="1481d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1481d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1481d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1481d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="1481d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1481d-120">Request headers</span></span>
|<span data-ttu-id="1481d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1481d-121">Header</span></span>|<span data-ttu-id="1481d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1481d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1481d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1481d-123">Authorization</span></span>|<span data-ttu-id="1481d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1481d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1481d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1481d-125">Accept</span></span>|<span data-ttu-id="1481d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1481d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1481d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1481d-127">Request body</span></span>
<span data-ttu-id="1481d-128">В тексте запроса добавьте представление объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1481d-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="1481d-129">В следующей таблице приведены свойства, необходимые при создании [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="1481d-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="1481d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1481d-130">Property</span></span>|<span data-ttu-id="1481d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1481d-131">Type</span></span>|<span data-ttu-id="1481d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1481d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1481d-133">id</span><span class="sxs-lookup"><span data-stu-id="1481d-133">id</span></span>|<span data-ttu-id="1481d-134">String</span><span class="sxs-lookup"><span data-stu-id="1481d-134">String</span></span>|<span data-ttu-id="1481d-135">Уникальный идентификатор для состояния работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="1481d-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="1481d-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1481d-136">This property is read-only.</span></span>|
|<span data-ttu-id="1481d-137">healthState</span><span class="sxs-lookup"><span data-stu-id="1481d-137">healthState</span></span>|[<span data-ttu-id="1481d-138">healthState</span><span class="sxs-lookup"><span data-stu-id="1481d-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="1481d-139">Состояние работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="1481d-139">Windows management app health state.</span></span> <span data-ttu-id="1481d-140">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="1481d-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="1481d-141">инсталледверсион</span><span class="sxs-lookup"><span data-stu-id="1481d-141">installedVersion</span></span>|<span data-ttu-id="1481d-142">String</span><span class="sxs-lookup"><span data-stu-id="1481d-142">String</span></span>|<span data-ttu-id="1481d-143">Установленная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="1481d-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="1481d-144">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="1481d-144">lastCheckInDateTime</span></span>|<span data-ttu-id="1481d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1481d-145">DateTimeOffset</span></span>|<span data-ttu-id="1481d-146">Время последнего возврата приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="1481d-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="1481d-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="1481d-147">deviceName</span></span>|<span data-ttu-id="1481d-148">String</span><span class="sxs-lookup"><span data-stu-id="1481d-148">String</span></span>|<span data-ttu-id="1481d-149">Имя устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="1481d-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="1481d-150">девицеосверсион</span><span class="sxs-lookup"><span data-stu-id="1481d-150">deviceOSVersion</span></span>|<span data-ttu-id="1481d-151">String</span><span class="sxs-lookup"><span data-stu-id="1481d-151">String</span></span>|<span data-ttu-id="1481d-152">Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="1481d-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="1481d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="1481d-153">Response</span></span>
<span data-ttu-id="1481d-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1481d-154">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1481d-155">Пример</span><span class="sxs-lookup"><span data-stu-id="1481d-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="1481d-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="1481d-156">Request</span></span>
<span data-ttu-id="1481d-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1481d-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### <a name="response"></a><span data-ttu-id="1481d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="1481d-158">Response</span></span>
<span data-ttu-id="1481d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1481d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
  "healthState": "healthy",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```






