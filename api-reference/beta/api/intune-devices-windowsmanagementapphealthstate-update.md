---
title: Обновление Виндовсманажементапфеалсстате
description: Обновление свойств объекта Виндовсманажементапфеалсстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4f956dc8ef3a1c4d65629d451396e274ae45f00
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944218"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="105af-103">Обновление Виндовсманажементапфеалсстате</span><span class="sxs-lookup"><span data-stu-id="105af-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="105af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="105af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="105af-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="105af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="105af-106">Обновление свойств объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="105af-106">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="105af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="105af-107">Prerequisites</span></span>
<span data-ttu-id="105af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="105af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="105af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="105af-110">Permission type</span></span>|<span data-ttu-id="105af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="105af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="105af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="105af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="105af-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="105af-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="105af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="105af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="105af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="105af-115">Not supported.</span></span>|
|<span data-ttu-id="105af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="105af-116">Application</span></span>|<span data-ttu-id="105af-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="105af-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="105af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="105af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="105af-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="105af-119">Request headers</span></span>
|<span data-ttu-id="105af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="105af-120">Header</span></span>|<span data-ttu-id="105af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="105af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="105af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="105af-122">Authorization</span></span>|<span data-ttu-id="105af-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="105af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="105af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="105af-124">Accept</span></span>|<span data-ttu-id="105af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="105af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="105af-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="105af-126">Request body</span></span>
<span data-ttu-id="105af-127">В тексте запроса добавьте представление объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="105af-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="105af-128">В следующей таблице приведены свойства, необходимые при создании [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="105af-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="105af-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="105af-129">Property</span></span>|<span data-ttu-id="105af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="105af-130">Type</span></span>|<span data-ttu-id="105af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="105af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="105af-132">id</span><span class="sxs-lookup"><span data-stu-id="105af-132">id</span></span>|<span data-ttu-id="105af-133">Строка</span><span class="sxs-lookup"><span data-stu-id="105af-133">String</span></span>|<span data-ttu-id="105af-134">Уникальный идентификатор для состояния работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="105af-134">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="105af-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="105af-135">This property is read-only.</span></span>|
|<span data-ttu-id="105af-136">healthState</span><span class="sxs-lookup"><span data-stu-id="105af-136">healthState</span></span>|[<span data-ttu-id="105af-137">healthState</span><span class="sxs-lookup"><span data-stu-id="105af-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="105af-138">Состояние работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="105af-138">Windows management app health state.</span></span> <span data-ttu-id="105af-139">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="105af-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="105af-140">инсталледверсион</span><span class="sxs-lookup"><span data-stu-id="105af-140">installedVersion</span></span>|<span data-ttu-id="105af-141">Строка</span><span class="sxs-lookup"><span data-stu-id="105af-141">String</span></span>|<span data-ttu-id="105af-142">Установленная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="105af-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="105af-143">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="105af-143">lastCheckInDateTime</span></span>|<span data-ttu-id="105af-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="105af-144">DateTimeOffset</span></span>|<span data-ttu-id="105af-145">Время последнего возврата приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="105af-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="105af-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="105af-146">deviceName</span></span>|<span data-ttu-id="105af-147">String</span><span class="sxs-lookup"><span data-stu-id="105af-147">String</span></span>|<span data-ttu-id="105af-148">Имя устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="105af-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="105af-149">девицеосверсион</span><span class="sxs-lookup"><span data-stu-id="105af-149">deviceOSVersion</span></span>|<span data-ttu-id="105af-150">Строка</span><span class="sxs-lookup"><span data-stu-id="105af-150">String</span></span>|<span data-ttu-id="105af-151">Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="105af-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="105af-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="105af-152">Response</span></span>
<span data-ttu-id="105af-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="105af-153">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="105af-154">Пример</span><span class="sxs-lookup"><span data-stu-id="105af-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="105af-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="105af-155">Request</span></span>
<span data-ttu-id="105af-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="105af-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="105af-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="105af-157">Response</span></span>
<span data-ttu-id="105af-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="105af-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





