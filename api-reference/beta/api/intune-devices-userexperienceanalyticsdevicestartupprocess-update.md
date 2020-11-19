---
title: Обновление Усерекспериенцеаналитиксдевицестартуппроцесс
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуппроцесс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 391060bb547aa4d2ab578d0f0a9b9215e3f23326
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49263878"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="fe836-103">Обновление Усерекспериенцеаналитиксдевицестартуппроцесс</span><span class="sxs-lookup"><span data-stu-id="fe836-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="fe836-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe836-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe836-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe836-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe836-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe836-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe836-107">Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="fe836-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe836-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe836-108">Prerequisites</span></span>
<span data-ttu-id="fe836-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe836-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe836-111">Permission type</span></span>|<span data-ttu-id="fe836-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe836-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe836-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe836-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe836-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe836-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe836-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe836-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe836-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe836-116">Not supported.</span></span>|
|<span data-ttu-id="fe836-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe836-117">Application</span></span>|<span data-ttu-id="fe836-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe836-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe836-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe836-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="fe836-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe836-120">Request headers</span></span>
|<span data-ttu-id="fe836-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe836-121">Header</span></span>|<span data-ttu-id="fe836-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe836-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe836-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe836-123">Authorization</span></span>|<span data-ttu-id="fe836-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe836-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe836-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe836-125">Accept</span></span>|<span data-ttu-id="fe836-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe836-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe836-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe836-127">Request body</span></span>
<span data-ttu-id="fe836-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe836-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="fe836-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span><span class="sxs-lookup"><span data-stu-id="fe836-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="fe836-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe836-130">Property</span></span>|<span data-ttu-id="fe836-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe836-131">Type</span></span>|<span data-ttu-id="fe836-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe836-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe836-133">id</span><span class="sxs-lookup"><span data-stu-id="fe836-133">id</span></span>|<span data-ttu-id="fe836-134">String</span><span class="sxs-lookup"><span data-stu-id="fe836-134">String</span></span>|<span data-ttu-id="fe836-135">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe836-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="fe836-136">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="fe836-136">managedDeviceId</span></span>|<span data-ttu-id="fe836-137">String</span><span class="sxs-lookup"><span data-stu-id="fe836-137">String</span></span>|<span data-ttu-id="fe836-138">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe836-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="fe836-139">процесснаме</span><span class="sxs-lookup"><span data-stu-id="fe836-139">processName</span></span>|<span data-ttu-id="fe836-140">String</span><span class="sxs-lookup"><span data-stu-id="fe836-140">String</span></span>|<span data-ttu-id="fe836-141">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe836-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="fe836-142">productName</span><span class="sxs-lookup"><span data-stu-id="fe836-142">productName</span></span>|<span data-ttu-id="fe836-143">String</span><span class="sxs-lookup"><span data-stu-id="fe836-143">String</span></span>|<span data-ttu-id="fe836-144">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="fe836-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="fe836-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fe836-145">publisher</span></span>|<span data-ttu-id="fe836-146">String</span><span class="sxs-lookup"><span data-stu-id="fe836-146">String</span></span>|<span data-ttu-id="fe836-147">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="fe836-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="fe836-148">стартупимпактинмс</span><span class="sxs-lookup"><span data-stu-id="fe836-148">startupImpactInMs</span></span>|<span data-ttu-id="fe836-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fe836-149">Int32</span></span>|<span data-ttu-id="fe836-150">Влияние процесса запуска пользователя на устройство Analytics в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="fe836-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="fe836-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe836-151">Response</span></span>
<span data-ttu-id="fe836-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe836-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe836-153">Пример</span><span class="sxs-lookup"><span data-stu-id="fe836-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe836-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe836-154">Request</span></span>
<span data-ttu-id="fe836-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe836-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe836-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe836-156">Response</span></span>
<span data-ttu-id="fe836-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe836-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




