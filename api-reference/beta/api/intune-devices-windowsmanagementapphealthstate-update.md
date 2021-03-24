---
title: Обновление windowsManagementAppHealthState
description: Обновление свойств объекта windowsManagementAppHealthState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88bfa7732662a1a3d2d0f7b60835a3a83bde90ad
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126327"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="d4522-103">Обновление windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="d4522-103">Update windowsManagementAppHealthState</span></span>

<span data-ttu-id="d4522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4522-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4522-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4522-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4522-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4522-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4522-107">Обновление свойств объекта [windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4522-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4522-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4522-108">Prerequisites</span></span>
<span data-ttu-id="d4522-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4522-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4522-111">Permission type</span></span>|<span data-ttu-id="d4522-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4522-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4522-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4522-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4522-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4522-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d4522-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4522-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4522-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4522-116">Not supported.</span></span>|
|<span data-ttu-id="d4522-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4522-117">Application</span></span>|<span data-ttu-id="d4522-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4522-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4522-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4522-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d4522-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4522-120">Request headers</span></span>
|<span data-ttu-id="d4522-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4522-121">Header</span></span>|<span data-ttu-id="d4522-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4522-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4522-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4522-123">Authorization</span></span>|<span data-ttu-id="d4522-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4522-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4522-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4522-125">Accept</span></span>|<span data-ttu-id="d4522-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4522-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4522-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4522-127">Request body</span></span>
<span data-ttu-id="d4522-128">В теле запроса укажи представление JSON для [объекта WindowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4522-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="d4522-129">В следующей таблице показаны свойства, необходимые при создании [windowsManagementAppHealthState.](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4522-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="d4522-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4522-130">Property</span></span>|<span data-ttu-id="d4522-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4522-131">Type</span></span>|<span data-ttu-id="d4522-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4522-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4522-133">id</span><span class="sxs-lookup"><span data-stu-id="d4522-133">id</span></span>|<span data-ttu-id="d4522-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d4522-134">String</span></span>|<span data-ttu-id="d4522-135">Уникальный идентификатор для состояния здоровья приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d4522-135">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="d4522-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4522-136">This property is read-only.</span></span>|
|<span data-ttu-id="d4522-137">healthState</span><span class="sxs-lookup"><span data-stu-id="d4522-137">healthState</span></span>|[<span data-ttu-id="d4522-138">healthState</span><span class="sxs-lookup"><span data-stu-id="d4522-138">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="d4522-139">Состояние здоровья приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d4522-139">Windows management app health state.</span></span> <span data-ttu-id="d4522-140">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="d4522-140">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="d4522-141">installedVersion</span><span class="sxs-lookup"><span data-stu-id="d4522-141">installedVersion</span></span>|<span data-ttu-id="d4522-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d4522-142">String</span></span>|<span data-ttu-id="d4522-143">Установленная версия приложения для управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d4522-143">Windows management app installed version.</span></span>|
|<span data-ttu-id="d4522-144">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="d4522-144">lastCheckInDateTime</span></span>|<span data-ttu-id="d4522-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4522-145">DateTimeOffset</span></span>|<span data-ttu-id="d4522-146">Приложение для управления Windows во время последней проверки.</span><span class="sxs-lookup"><span data-stu-id="d4522-146">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="d4522-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="d4522-147">deviceName</span></span>|<span data-ttu-id="d4522-148">String</span><span class="sxs-lookup"><span data-stu-id="d4522-148">String</span></span>|<span data-ttu-id="d4522-149">Имя устройства, на котором установлено приложение для управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d4522-149">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="d4522-150">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="d4522-150">deviceOSVersion</span></span>|<span data-ttu-id="d4522-151">Строка</span><span class="sxs-lookup"><span data-stu-id="d4522-151">String</span></span>|<span data-ttu-id="d4522-152">Windows 10 ОС версии устройства, на котором установлено приложение для управления Windows.</span><span class="sxs-lookup"><span data-stu-id="d4522-152">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="d4522-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4522-153">Response</span></span>
<span data-ttu-id="d4522-154">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4522-154">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4522-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d4522-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4522-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4522-156">Request</span></span>
<span data-ttu-id="d4522-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4522-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4522-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4522-158">Response</span></span>
<span data-ttu-id="d4522-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4522-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




