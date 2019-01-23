---
title: Обновление windowsManagementAppHealthState
description: Обновление свойства объекта windowsManagementAppHealthState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: de395bdeba104ea3c5c30b8f33e8670a5f2e5480
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423155"
---
# <a name="update-windowsmanagementapphealthstate"></a><span data-ttu-id="e906e-103">Обновление windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="e906e-103">Update windowsManagementAppHealthState</span></span>

> <span data-ttu-id="e906e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e906e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e906e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e906e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e906e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e906e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e906e-107">Обновление свойства объекта [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="e906e-107">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e906e-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e906e-108">Prerequisites</span></span>
<span data-ttu-id="e906e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e906e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e906e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e906e-111">Permission type</span></span>|<span data-ttu-id="e906e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e906e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e906e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e906e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e906e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e906e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e906e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e906e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e906e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e906e-116">Not supported.</span></span>|
|<span data-ttu-id="e906e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e906e-117">Application</span></span>|<span data-ttu-id="e906e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e906e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e906e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e906e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e906e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e906e-120">Request headers</span></span>
|<span data-ttu-id="e906e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e906e-121">Header</span></span>|<span data-ttu-id="e906e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e906e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e906e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e906e-123">Authorization</span></span>|<span data-ttu-id="e906e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e906e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e906e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e906e-125">Accept</span></span>|<span data-ttu-id="e906e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e906e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e906e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e906e-127">Request body</span></span>
<span data-ttu-id="e906e-128">В тексте запроса укажите представление JSON для объекта [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="e906e-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>

<span data-ttu-id="e906e-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span><span class="sxs-lookup"><span data-stu-id="e906e-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>

|<span data-ttu-id="e906e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e906e-130">Property</span></span>|<span data-ttu-id="e906e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e906e-131">Type</span></span>|<span data-ttu-id="e906e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e906e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e906e-133">id</span><span class="sxs-lookup"><span data-stu-id="e906e-133">id</span></span>|<span data-ttu-id="e906e-134">String</span><span class="sxs-lookup"><span data-stu-id="e906e-134">String</span></span>|<span data-ttu-id="e906e-135">Уникальный идентификатор для состояния работоспособности приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="e906e-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="e906e-136">healthState</span><span class="sxs-lookup"><span data-stu-id="e906e-136">healthState</span></span>|[<span data-ttu-id="e906e-137">healthState</span><span class="sxs-lookup"><span data-stu-id="e906e-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="e906e-138">Состояния работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="e906e-138">Windows management app health state.</span></span> <span data-ttu-id="e906e-139">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="e906e-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="e906e-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="e906e-140">installedVersion</span></span>|<span data-ttu-id="e906e-141">String</span><span class="sxs-lookup"><span data-stu-id="e906e-141">String</span></span>|<span data-ttu-id="e906e-142">Управление приложения установленной версии Windows.</span><span class="sxs-lookup"><span data-stu-id="e906e-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="e906e-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="e906e-143">lastCheckInDateTime</span></span>|<span data-ttu-id="e906e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e906e-144">DateTimeOffset</span></span>|<span data-ttu-id="e906e-145">Приложение управления Windows последний раз.</span><span class="sxs-lookup"><span data-stu-id="e906e-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="e906e-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="e906e-146">deviceName</span></span>|<span data-ttu-id="e906e-147">String</span><span class="sxs-lookup"><span data-stu-id="e906e-147">String</span></span>|<span data-ttu-id="e906e-148">Имя устройства, на какие Windows установлено приложение управления.</span><span class="sxs-lookup"><span data-stu-id="e906e-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="e906e-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="e906e-149">deviceOSVersion</span></span>|<span data-ttu-id="e906e-150">String</span><span class="sxs-lookup"><span data-stu-id="e906e-150">String</span></span>|<span data-ttu-id="e906e-151">10 версии Windows устройства, на какие Windows установлено приложение управления.</span><span class="sxs-lookup"><span data-stu-id="e906e-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="e906e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e906e-152">Response</span></span>
<span data-ttu-id="e906e-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e906e-153">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e906e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e906e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e906e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="e906e-155">Request</span></span>
<span data-ttu-id="e906e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e906e-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e906e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e906e-157">Response</span></span>
<span data-ttu-id="e906e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e906e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




