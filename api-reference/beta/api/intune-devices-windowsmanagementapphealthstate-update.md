---
title: Обновление Виндовсманажементапфеалсстате
description: Обновление свойств объекта Виндовсманажементапфеалсстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58ea766e7776f88f55d6cd7dad2bd9e01e38bd46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534264"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="88e57-103">Обновление Виндовсманажементапфеалсстате</span><span class="sxs-lookup"><span data-stu-id="88e57-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="88e57-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88e57-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88e57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88e57-106">Обновление свойств объекта [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="88e57-106">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88e57-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88e57-107">Prerequisites</span></span>
<span data-ttu-id="88e57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e57-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88e57-110">Permission type</span></span>|<span data-ttu-id="88e57-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88e57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88e57-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88e57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88e57-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e57-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88e57-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88e57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88e57-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e57-115">Not supported.</span></span>|
|<span data-ttu-id="88e57-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88e57-116">Application</span></span>|<span data-ttu-id="88e57-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88e57-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88e57-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88e57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="88e57-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88e57-119">Request headers</span></span>
|<span data-ttu-id="88e57-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88e57-120">Header</span></span>|<span data-ttu-id="88e57-121">Значение</span><span class="sxs-lookup"><span data-stu-id="88e57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88e57-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88e57-122">Authorization</span></span>|<span data-ttu-id="88e57-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88e57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88e57-124">Accept</span><span class="sxs-lookup"><span data-stu-id="88e57-124">Accept</span></span>|<span data-ttu-id="88e57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88e57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88e57-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88e57-126">Request body</span></span>
<span data-ttu-id="88e57-127">В тексте запроса добавьте представление объекта [Виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88e57-127">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="88e57-128">В следующей таблице приведены свойства, необходимые при создании [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="88e57-128">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="88e57-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="88e57-129">Property</span></span>|<span data-ttu-id="88e57-130">Тип</span><span class="sxs-lookup"><span data-stu-id="88e57-130">Type</span></span>|<span data-ttu-id="88e57-131">Описание</span><span class="sxs-lookup"><span data-stu-id="88e57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88e57-132">id</span><span class="sxs-lookup"><span data-stu-id="88e57-132">id</span></span>|<span data-ttu-id="88e57-133">String</span><span class="sxs-lookup"><span data-stu-id="88e57-133">String</span></span>|<span data-ttu-id="88e57-134">Уникальный идентификатор для состояния работоспособности приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="88e57-134">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="88e57-135">healthState</span><span class="sxs-lookup"><span data-stu-id="88e57-135">healthState</span></span>|[<span data-ttu-id="88e57-136">healthState</span><span class="sxs-lookup"><span data-stu-id="88e57-136">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="88e57-137">Состояние работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="88e57-137">Windows management app health state.</span></span> <span data-ttu-id="88e57-138">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="88e57-138">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="88e57-139">Инсталледверсион</span><span class="sxs-lookup"><span data-stu-id="88e57-139">installedVersion</span></span>|<span data-ttu-id="88e57-140">String</span><span class="sxs-lookup"><span data-stu-id="88e57-140">String</span></span>|<span data-ttu-id="88e57-141">Установленная версия приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="88e57-141">Windows management app installed version.</span></span>|
|<span data-ttu-id="88e57-142">Ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="88e57-142">lastCheckInDateTime</span></span>|<span data-ttu-id="88e57-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88e57-143">DateTimeOffset</span></span>|<span data-ttu-id="88e57-144">Время последнего возврата приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="88e57-144">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="88e57-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="88e57-145">deviceName</span></span>|<span data-ttu-id="88e57-146">String</span><span class="sxs-lookup"><span data-stu-id="88e57-146">String</span></span>|<span data-ttu-id="88e57-147">Имя устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="88e57-147">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="88e57-148">Девицеосверсион</span><span class="sxs-lookup"><span data-stu-id="88e57-148">deviceOSVersion</span></span>|<span data-ttu-id="88e57-149">String</span><span class="sxs-lookup"><span data-stu-id="88e57-149">String</span></span>|<span data-ttu-id="88e57-150">Версия Windows 10 OS устройства, на котором установлено приложение "Управление Windows".</span><span class="sxs-lookup"><span data-stu-id="88e57-150">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="88e57-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="88e57-151">Response</span></span>
<span data-ttu-id="88e57-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсманажементапфеалсстате](../resources/intune-devices-windowsmanagementapphealthstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88e57-152">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88e57-153">Пример</span><span class="sxs-lookup"><span data-stu-id="88e57-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="88e57-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="88e57-154">Request</span></span>
<span data-ttu-id="88e57-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88e57-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88e57-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="88e57-156">Response</span></span>
<span data-ttu-id="88e57-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88e57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





