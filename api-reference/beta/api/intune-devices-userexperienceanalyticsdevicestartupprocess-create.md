---
title: Создание userExperienceAnalyticsDeviceStartupProcess
description: Создание нового объекта userExperienceAnalyticsDeviceStartupProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e269a9ad65db24f3646e49ab80d11edbaeb1952
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135994"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="087cf-103">Создание userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="087cf-103">Create userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="087cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="087cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="087cf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="087cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="087cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="087cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="087cf-107">Создание нового [объекта userExperienceAnalyticsDeviceStartupProcess.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)</span><span class="sxs-lookup"><span data-stu-id="087cf-107">Create a new [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="087cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="087cf-108">Prerequisites</span></span>
<span data-ttu-id="087cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="087cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="087cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="087cf-111">Permission type</span></span>|<span data-ttu-id="087cf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="087cf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="087cf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="087cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="087cf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="087cf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="087cf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="087cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="087cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="087cf-116">Not supported.</span></span>|
|<span data-ttu-id="087cf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="087cf-117">Application</span></span>|<span data-ttu-id="087cf-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="087cf-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="087cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="087cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="087cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="087cf-120">Request headers</span></span>
|<span data-ttu-id="087cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="087cf-121">Header</span></span>|<span data-ttu-id="087cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="087cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="087cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="087cf-123">Authorization</span></span>|<span data-ttu-id="087cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="087cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="087cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="087cf-125">Accept</span></span>|<span data-ttu-id="087cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="087cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="087cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="087cf-127">Request body</span></span>
<span data-ttu-id="087cf-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsDeviceStartupProcess.</span><span class="sxs-lookup"><span data-stu-id="087cf-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcess object.</span></span>

<span data-ttu-id="087cf-129">В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsDeviceStartupProcess.</span><span class="sxs-lookup"><span data-stu-id="087cf-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcess.</span></span>

|<span data-ttu-id="087cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="087cf-130">Property</span></span>|<span data-ttu-id="087cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="087cf-131">Type</span></span>|<span data-ttu-id="087cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="087cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="087cf-133">id</span><span class="sxs-lookup"><span data-stu-id="087cf-133">id</span></span>|<span data-ttu-id="087cf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="087cf-134">String</span></span>|<span data-ttu-id="087cf-135">Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="087cf-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="087cf-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="087cf-136">managedDeviceId</span></span>|<span data-ttu-id="087cf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="087cf-137">String</span></span>|<span data-ttu-id="087cf-138">ID устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="087cf-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="087cf-139">processName</span><span class="sxs-lookup"><span data-stu-id="087cf-139">processName</span></span>|<span data-ttu-id="087cf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="087cf-140">String</span></span>|<span data-ttu-id="087cf-141">Имя процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="087cf-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="087cf-142">productName</span><span class="sxs-lookup"><span data-stu-id="087cf-142">productName</span></span>|<span data-ttu-id="087cf-143">String</span><span class="sxs-lookup"><span data-stu-id="087cf-143">String</span></span>|<span data-ttu-id="087cf-144">Имя продукта процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="087cf-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="087cf-145">publisher</span><span class="sxs-lookup"><span data-stu-id="087cf-145">publisher</span></span>|<span data-ttu-id="087cf-146">String</span><span class="sxs-lookup"><span data-stu-id="087cf-146">String</span></span>|<span data-ttu-id="087cf-147">Издатель процесса запуска устройства для аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="087cf-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="087cf-148">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="087cf-148">startupImpactInMs</span></span>|<span data-ttu-id="087cf-149">Int32</span><span class="sxs-lookup"><span data-stu-id="087cf-149">Int32</span></span>|<span data-ttu-id="087cf-150">Влияние процесса запуска устройства для аналитики пользовательских интерфейсов в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="087cf-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="087cf-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="087cf-151">Response</span></span>
<span data-ttu-id="087cf-152">В случае успеха этот метод возвращает код ответа и объект `201 Created` [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="087cf-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="087cf-153">Пример</span><span class="sxs-lookup"><span data-stu-id="087cf-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="087cf-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="087cf-154">Request</span></span>
<span data-ttu-id="087cf-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="087cf-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
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

### <a name="response"></a><span data-ttu-id="087cf-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="087cf-156">Response</span></span>
<span data-ttu-id="087cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="087cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




