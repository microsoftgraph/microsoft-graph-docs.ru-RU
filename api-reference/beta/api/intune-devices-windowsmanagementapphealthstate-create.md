---
title: Создание Виндовсманажементапфеалсстате
description: Создание нового объекта Виндовсманажементапфеалсстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96f6b3e66055e06424c367e177f4cbb42b322c77
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37526458"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="8308e-103">Создание Виндовсманажементапфеалсстате</span><span class="sxs-lookup"><span data-stu-id="8308e-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="8308e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8308e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8308e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8308e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8308e-106">Создание нового объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="8308e-106">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8308e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8308e-107">Prerequisites</span></span>
<span data-ttu-id="8308e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8308e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8308e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8308e-110">Permission type</span></span>|<span data-ttu-id="8308e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8308e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8308e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8308e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8308e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8308e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8308e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8308e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8308e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8308e-115">Not supported.</span></span>|
|<span data-ttu-id="8308e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8308e-116">Application</span></span>|<span data-ttu-id="8308e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8308e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8308e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8308e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="8308e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8308e-119">Request headers</span></span>
|<span data-ttu-id="8308e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8308e-120">Header</span></span>|<span data-ttu-id="8308e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8308e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8308e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8308e-122">Authorization</span></span>|<span data-ttu-id="8308e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8308e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8308e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8308e-124">Accept</span></span>|<span data-ttu-id="8308e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8308e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8308e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8308e-126">Request body</span></span>
<span data-ttu-id="8308e-127">В тексте запроса добавьте представление объекта Виндовсманажементапфеалсстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8308e-127">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="8308e-128">В следующей таблице приведены свойства, необходимые при создании Виндовсманажементапфеалсстате.</span><span class="sxs-lookup"><span data-stu-id="8308e-128">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="8308e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8308e-129">Property</span></span>|<span data-ttu-id="8308e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8308e-130">Type</span></span>|<span data-ttu-id="8308e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8308e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8308e-132">id</span><span class="sxs-lookup"><span data-stu-id="8308e-132">id</span></span>|<span data-ttu-id="8308e-133">String</span><span class="sxs-lookup"><span data-stu-id="8308e-133">String</span></span>|<span data-ttu-id="8308e-134">Уникальный идентификатор для состояния работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="8308e-134">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="8308e-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8308e-135">This property is read-only.</span></span>|
|<span data-ttu-id="8308e-136">healthState</span><span class="sxs-lookup"><span data-stu-id="8308e-136">healthState</span></span>|[<span data-ttu-id="8308e-137">healthState</span><span class="sxs-lookup"><span data-stu-id="8308e-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="8308e-138">Состояние работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="8308e-138">Windows management app health state.</span></span> <span data-ttu-id="8308e-139">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="8308e-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="8308e-140">инсталледверсион</span><span class="sxs-lookup"><span data-stu-id="8308e-140">installedVersion</span></span>|<span data-ttu-id="8308e-141">String</span><span class="sxs-lookup"><span data-stu-id="8308e-141">String</span></span>|<span data-ttu-id="8308e-142">Установленная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="8308e-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="8308e-143">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="8308e-143">lastCheckInDateTime</span></span>|<span data-ttu-id="8308e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8308e-144">DateTimeOffset</span></span>|<span data-ttu-id="8308e-145">Время последнего возврата приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="8308e-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="8308e-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="8308e-146">deviceName</span></span>|<span data-ttu-id="8308e-147">String</span><span class="sxs-lookup"><span data-stu-id="8308e-147">String</span></span>|<span data-ttu-id="8308e-148">Имя устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="8308e-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="8308e-149">девицеосверсион</span><span class="sxs-lookup"><span data-stu-id="8308e-149">deviceOSVersion</span></span>|<span data-ttu-id="8308e-150">String</span><span class="sxs-lookup"><span data-stu-id="8308e-150">String</span></span>|<span data-ttu-id="8308e-151">Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="8308e-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="8308e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8308e-152">Response</span></span>
<span data-ttu-id="8308e-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8308e-153">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8308e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="8308e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="8308e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8308e-155">Request</span></span>
<span data-ttu-id="8308e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8308e-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8308e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="8308e-157">Response</span></span>
<span data-ttu-id="8308e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8308e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






