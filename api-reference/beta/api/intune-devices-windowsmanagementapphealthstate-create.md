---
title: Создание windowsManagementAppHealthState
description: Создание нового объекта windowsManagementAppHealthState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dce9b217b7234fadff0d8cbdc962f1ef38e66c0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939001"
---
# <a name="create-windowsmanagementapphealthstate"></a><span data-ttu-id="45c32-103">Создание windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="45c32-103">Create windowsManagementAppHealthState</span></span>

> <span data-ttu-id="45c32-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45c32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45c32-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45c32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45c32-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45c32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45c32-107">Создание нового объекта [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) .</span><span class="sxs-lookup"><span data-stu-id="45c32-107">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45c32-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45c32-108">Prerequisites</span></span>
<span data-ttu-id="45c32-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45c32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45c32-111">Permission type</span></span>|<span data-ttu-id="45c32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45c32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45c32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45c32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45c32-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c32-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="45c32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45c32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45c32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45c32-116">Not supported.</span></span>|
|<span data-ttu-id="45c32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45c32-117">Application</span></span>|<span data-ttu-id="45c32-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45c32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45c32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45c32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="45c32-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45c32-120">Request headers</span></span>
|<span data-ttu-id="45c32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45c32-121">Header</span></span>|<span data-ttu-id="45c32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45c32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45c32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45c32-123">Authorization</span></span>|<span data-ttu-id="45c32-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45c32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45c32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45c32-125">Accept</span></span>|<span data-ttu-id="45c32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45c32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45c32-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45c32-127">Request body</span></span>
<span data-ttu-id="45c32-128">В тексте запроса укажите представление JSON для объекта windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="45c32-128">In the request body, supply a JSON representation for the windowsManagementAppHealthState object.</span></span>

<span data-ttu-id="45c32-129">В следующей таблице показаны свойства, которые необходимы для создания windowsManagementAppHealthState.</span><span class="sxs-lookup"><span data-stu-id="45c32-129">The following table shows the properties that are required when you create the windowsManagementAppHealthState.</span></span>

|<span data-ttu-id="45c32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="45c32-130">Property</span></span>|<span data-ttu-id="45c32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="45c32-131">Type</span></span>|<span data-ttu-id="45c32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="45c32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45c32-133">id</span><span class="sxs-lookup"><span data-stu-id="45c32-133">id</span></span>|<span data-ttu-id="45c32-134">Строка</span><span class="sxs-lookup"><span data-stu-id="45c32-134">String</span></span>|<span data-ttu-id="45c32-135">Уникальный идентификатор для состояния работоспособности приложения управления Windows</span><span class="sxs-lookup"><span data-stu-id="45c32-135">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="45c32-136">healthState</span><span class="sxs-lookup"><span data-stu-id="45c32-136">healthState</span></span>|[<span data-ttu-id="45c32-137">healthState</span><span class="sxs-lookup"><span data-stu-id="45c32-137">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="45c32-138">Состояния работоспособности приложения управления Windows.</span><span class="sxs-lookup"><span data-stu-id="45c32-138">Windows management app health state.</span></span> <span data-ttu-id="45c32-139">Возможные значения: `unknown`, `healthy`, `unhealthy`.</span><span class="sxs-lookup"><span data-stu-id="45c32-139">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="45c32-140">installedVersion</span><span class="sxs-lookup"><span data-stu-id="45c32-140">installedVersion</span></span>|<span data-ttu-id="45c32-141">Строка</span><span class="sxs-lookup"><span data-stu-id="45c32-141">String</span></span>|<span data-ttu-id="45c32-142">Управление приложения установленной версии Windows.</span><span class="sxs-lookup"><span data-stu-id="45c32-142">Windows management app installed version.</span></span>|
|<span data-ttu-id="45c32-143">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="45c32-143">lastCheckInDateTime</span></span>|<span data-ttu-id="45c32-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c32-144">DateTimeOffset</span></span>|<span data-ttu-id="45c32-145">Приложение управления Windows последний раз.</span><span class="sxs-lookup"><span data-stu-id="45c32-145">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="45c32-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="45c32-146">deviceName</span></span>|<span data-ttu-id="45c32-147">String</span><span class="sxs-lookup"><span data-stu-id="45c32-147">String</span></span>|<span data-ttu-id="45c32-148">Имя устройства, на какие Windows установлено приложение управления.</span><span class="sxs-lookup"><span data-stu-id="45c32-148">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="45c32-149">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="45c32-149">deviceOSVersion</span></span>|<span data-ttu-id="45c32-150">Строка</span><span class="sxs-lookup"><span data-stu-id="45c32-150">String</span></span>|<span data-ttu-id="45c32-151">10 версии Windows устройства, на какие Windows установлено приложение управления.</span><span class="sxs-lookup"><span data-stu-id="45c32-151">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|



## <a name="response"></a><span data-ttu-id="45c32-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="45c32-152">Response</span></span>
<span data-ttu-id="45c32-153">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45c32-153">If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c32-154">Пример</span><span class="sxs-lookup"><span data-stu-id="45c32-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="45c32-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="45c32-155">Request</span></span>
<span data-ttu-id="45c32-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45c32-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45c32-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="45c32-157">Response</span></span>
<span data-ttu-id="45c32-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45c32-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





