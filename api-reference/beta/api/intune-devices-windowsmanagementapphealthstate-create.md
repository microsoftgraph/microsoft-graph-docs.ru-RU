---
title: Создание Виндовсманажементапфеалсстате
description: Создание нового объекта Виндовсманажементапфеалсстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7995d21550b6152ec4fae020fd42e8118f334fb8
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944246"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="ee261-103">Создание Виндовсманажементапфеалсстате</span><span class="sxs-lookup"><span data-stu-id="ee261-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="ee261-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee261-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee261-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee261-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee261-106">Создание нового объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ee261-106">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee261-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee261-107">Prerequisites</span></span>
<span data-ttu-id="ee261-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee261-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee261-110">Permission type</span></span>|<span data-ttu-id="ee261-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee261-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee261-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee261-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee261-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee261-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee261-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee261-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee261-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee261-115">Not supported.</span></span>|
|<span data-ttu-id="ee261-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee261-116">Application</span></span>|<span data-ttu-id="ee261-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee261-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee261-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee261-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="ee261-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ee261-119">Request headers</span></span>
|<span data-ttu-id="ee261-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee261-120">Header</span></span>|<span data-ttu-id="ee261-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee261-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee261-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee261-122">Authorization</span></span>|<span data-ttu-id="ee261-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee261-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee261-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee261-124">Accept</span></span>|<span data-ttu-id="ee261-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee261-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee261-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee261-126">Request body</span></span>
<span data-ttu-id="ee261-127">В тексте запроса добавьте представление объекта Виндовсманажементапфеалсстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee261-127">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="ee261-128">В следующей таблице приведены свойства, необходимые при создании Виндовсманажементапфеалсстате.</span><span class="sxs-lookup"><span data-stu-id="ee261-128">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="ee261-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee261-129">Property</span></span>|<span data-ttu-id="ee261-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee261-130">Type</span></span>|<span data-ttu-id="ee261-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee261-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee261-132">id</span><span class="sxs-lookup"><span data-stu-id="ee261-132">id</span></span>|<span data-ttu-id="ee261-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ee261-133">String</span></span>|<span data-ttu-id="ee261-134">Уникальный идентификатор для состояния работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="ee261-134">Unique Identifier for the Windows management app health state.</span></span> <span data-ttu-id="ee261-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee261-135">This property is read-only.</span></span>|
|<span data-ttu-id="ee261-136">healthState</span><span class="sxs-lookup"><span data-stu-id="ee261-136">healthState</span></span>|[<span data-ttu-id="ee261-137">healthState</span><span class="sxs-lookup"><span data-stu-id="ee261-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="ee261-138">Состояние работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="ee261-138">Windows management app health state.</span></span> <span data-ttu-id="ee261-139">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="ee261-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="ee261-140">инсталледверсион</span><span class="sxs-lookup"><span data-stu-id="ee261-140">installedVersion</span></span>|<span data-ttu-id="ee261-141">Строка</span><span class="sxs-lookup"><span data-stu-id="ee261-141">String</span></span>|<span data-ttu-id="ee261-142">Установленная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="ee261-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="ee261-143">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="ee261-143">lastCheckInDateTime</span></span>|<span data-ttu-id="ee261-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee261-144">DateTimeOffset</span></span>|<span data-ttu-id="ee261-145">Время последнего возврата приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="ee261-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="ee261-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="ee261-146">deviceName</span></span>|<span data-ttu-id="ee261-147">String</span><span class="sxs-lookup"><span data-stu-id="ee261-147">String</span></span>|<span data-ttu-id="ee261-148">Имя устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="ee261-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="ee261-149">девицеосверсион</span><span class="sxs-lookup"><span data-stu-id="ee261-149">deviceOSVersion</span></span>|<span data-ttu-id="ee261-150">Строка</span><span class="sxs-lookup"><span data-stu-id="ee261-150">String</span></span>|<span data-ttu-id="ee261-151">Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="ee261-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="ee261-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee261-152">Response</span></span>
<span data-ttu-id="ee261-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee261-153">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee261-154">Пример</span><span class="sxs-lookup"><span data-stu-id="ee261-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee261-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee261-155">Request</span></span>
<span data-ttu-id="ee261-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee261-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee261-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee261-157">Response</span></span>
<span data-ttu-id="ee261-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee261-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





