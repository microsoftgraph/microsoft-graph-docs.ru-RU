---
title: Обновление userExperienceAnalyticsDeviceStartupProcess
description: Обновление свойств объекта userExperienceAnalyticsDeviceStartupProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8439c1ddcd646fc208950195224fc9241b4ae435
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154058"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="05664-103">Обновление userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="05664-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="05664-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05664-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05664-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05664-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05664-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05664-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05664-107">Обновление свойств объекта [userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="05664-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05664-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="05664-108">Prerequisites</span></span>
<span data-ttu-id="05664-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05664-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05664-111">Permission type</span></span>|<span data-ttu-id="05664-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05664-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05664-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05664-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05664-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05664-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="05664-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05664-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05664-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05664-116">Not supported.</span></span>|
|<span data-ttu-id="05664-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="05664-117">Application</span></span>|<span data-ttu-id="05664-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05664-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05664-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05664-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="05664-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="05664-120">Request headers</span></span>
|<span data-ttu-id="05664-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05664-121">Header</span></span>|<span data-ttu-id="05664-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05664-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05664-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05664-123">Authorization</span></span>|<span data-ttu-id="05664-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05664-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05664-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05664-125">Accept</span></span>|<span data-ttu-id="05664-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05664-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05664-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05664-127">Request body</span></span>
<span data-ttu-id="05664-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="05664-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="05664-129">В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="05664-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="05664-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="05664-130">Property</span></span>|<span data-ttu-id="05664-131">Тип</span><span class="sxs-lookup"><span data-stu-id="05664-131">Type</span></span>|<span data-ttu-id="05664-132">Описание</span><span class="sxs-lookup"><span data-stu-id="05664-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05664-133">id</span><span class="sxs-lookup"><span data-stu-id="05664-133">id</span></span>|<span data-ttu-id="05664-134">Строка</span><span class="sxs-lookup"><span data-stu-id="05664-134">String</span></span>|<span data-ttu-id="05664-135">Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="05664-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="05664-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="05664-136">managedDeviceId</span></span>|<span data-ttu-id="05664-137">Строка</span><span class="sxs-lookup"><span data-stu-id="05664-137">String</span></span>|<span data-ttu-id="05664-138">ID устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="05664-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="05664-139">processName</span><span class="sxs-lookup"><span data-stu-id="05664-139">processName</span></span>|<span data-ttu-id="05664-140">Строка</span><span class="sxs-lookup"><span data-stu-id="05664-140">String</span></span>|<span data-ttu-id="05664-141">Имя процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="05664-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="05664-142">productName</span><span class="sxs-lookup"><span data-stu-id="05664-142">productName</span></span>|<span data-ttu-id="05664-143">String</span><span class="sxs-lookup"><span data-stu-id="05664-143">String</span></span>|<span data-ttu-id="05664-144">Имя продукта процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="05664-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="05664-145">publisher</span><span class="sxs-lookup"><span data-stu-id="05664-145">publisher</span></span>|<span data-ttu-id="05664-146">String</span><span class="sxs-lookup"><span data-stu-id="05664-146">String</span></span>|<span data-ttu-id="05664-147">Издатель процесса запуска устройства для аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="05664-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="05664-148">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="05664-148">startupImpactInMs</span></span>|<span data-ttu-id="05664-149">Int32</span><span class="sxs-lookup"><span data-stu-id="05664-149">Int32</span></span>|<span data-ttu-id="05664-150">Влияние процесса запуска устройства для аналитики пользовательских интерфейсов в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="05664-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="05664-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="05664-151">Response</span></span>
<span data-ttu-id="05664-152">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsDeviceStartupProcess в](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="05664-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05664-153">Пример</span><span class="sxs-lookup"><span data-stu-id="05664-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="05664-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="05664-154">Request</span></span>
<span data-ttu-id="05664-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05664-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
Content-type: application/json
Content-length: 276

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```

### <a name="response"></a><span data-ttu-id="05664-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="05664-156">Response</span></span>
<span data-ttu-id="05664-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05664-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "03b451e6-51e6-03b4-e651-b403e651b403",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```




