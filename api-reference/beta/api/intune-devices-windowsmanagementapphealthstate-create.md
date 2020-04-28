---
title: Создание Виндовсманажементапфеалсстате
description: Создание нового объекта Виндовсманажементапфеалсстате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9514f00e5044baf1faf64fc9a15833fb8c7f975
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43321571"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="4090f-103">Создание Виндовсманажементапфеалсстате</span><span class="sxs-lookup"><span data-stu-id="4090f-103">Create windowsManagementAppHealthState</span></span>

<span data-ttu-id="4090f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4090f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4090f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4090f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4090f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4090f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4090f-107">Создание нового объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="4090f-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4090f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4090f-108">Prerequisites</span></span>
<span data-ttu-id="4090f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4090f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4090f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4090f-111">Permission type</span></span>|<span data-ttu-id="4090f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4090f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4090f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4090f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4090f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4090f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4090f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4090f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4090f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4090f-116">Not supported.</span></span>|
|<span data-ttu-id="4090f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4090f-117">Application</span></span>|<span data-ttu-id="4090f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4090f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4090f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4090f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="4090f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4090f-120">Request headers</span></span>
|<span data-ttu-id="4090f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4090f-121">Header</span></span>|<span data-ttu-id="4090f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4090f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4090f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4090f-123">Authorization</span></span>|<span data-ttu-id="4090f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4090f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4090f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4090f-125">Accept</span></span>|<span data-ttu-id="4090f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4090f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4090f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4090f-127">Request body</span></span>
<span data-ttu-id="4090f-128">В тексте запроса добавьте представление объекта Виндовсманажементапфеалсстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4090f-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="4090f-129">В следующей таблице приведены свойства, необходимые при создании Виндовсманажементапфеалсстате.</span><span class="sxs-lookup"><span data-stu-id="4090f-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="4090f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4090f-130">Property</span></span>|<span data-ttu-id="4090f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4090f-131">Type</span></span>|<span data-ttu-id="4090f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4090f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4090f-133">id</span><span class="sxs-lookup"><span data-stu-id="4090f-133">id</span></span>|<span data-ttu-id="4090f-134">String</span><span class="sxs-lookup"><span data-stu-id="4090f-134">String</span></span>|<span data-ttu-id="4090f-135">Уникальный идентификатор для состояния работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="4090f-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="4090f-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4090f-136">This property is read-only.</span></span>|
|<span data-ttu-id="4090f-137">healthState</span><span class="sxs-lookup"><span data-stu-id="4090f-137">healthState</span></span>|[<span data-ttu-id="4090f-138">healthState</span><span class="sxs-lookup"><span data-stu-id="4090f-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="4090f-139">Состояние работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="4090f-139">Windows management app health state.</span></span> <span data-ttu-id="4090f-140">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="4090f-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="4090f-141">инсталледверсион</span><span class="sxs-lookup"><span data-stu-id="4090f-141">installedVersion</span></span>|<span data-ttu-id="4090f-142">String</span><span class="sxs-lookup"><span data-stu-id="4090f-142">String</span></span>|<span data-ttu-id="4090f-143">Установленная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="4090f-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="4090f-144">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="4090f-144">lastCheckInDateTime</span></span>|<span data-ttu-id="4090f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4090f-145">DateTimeOffset</span></span>|<span data-ttu-id="4090f-146">Время последнего возврата приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="4090f-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="4090f-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="4090f-147">deviceName</span></span>|<span data-ttu-id="4090f-148">String</span><span class="sxs-lookup"><span data-stu-id="4090f-148">String</span></span>|<span data-ttu-id="4090f-149">Имя устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="4090f-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="4090f-150">девицеосверсион</span><span class="sxs-lookup"><span data-stu-id="4090f-150">deviceOSVersion</span></span>|<span data-ttu-id="4090f-151">String</span><span class="sxs-lookup"><span data-stu-id="4090f-151">String</span></span>|<span data-ttu-id="4090f-152">Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="4090f-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="4090f-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="4090f-153">Response</span></span>
<span data-ttu-id="4090f-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4090f-154">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4090f-155">Пример</span><span class="sxs-lookup"><span data-stu-id="4090f-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="4090f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4090f-156">Request</span></span>
<span data-ttu-id="4090f-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4090f-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
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

### <a name="response"></a><span data-ttu-id="4090f-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4090f-158">Response</span></span>
<span data-ttu-id="4090f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4090f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



