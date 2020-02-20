---
title: Обновление Усерекспериенцеаналитиксдевицестартуппроцесс
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуппроцесс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe146e97c6807287fadc265f9a9492ff03c03d9d
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161989"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="f3637-103">Обновление Усерекспериенцеаналитиксдевицестартуппроцесс</span><span class="sxs-lookup"><span data-stu-id="f3637-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="f3637-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3637-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3637-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3637-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3637-106">Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="f3637-106">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3637-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3637-107">Prerequisites</span></span>
<span data-ttu-id="f3637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3637-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3637-110">Permission type</span></span>|<span data-ttu-id="f3637-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3637-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3637-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3637-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3637-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3637-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3637-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3637-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3637-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3637-115">Not supported.</span></span>|
|<span data-ttu-id="f3637-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3637-116">Application</span></span>|<span data-ttu-id="f3637-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3637-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3637-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3637-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="f3637-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3637-119">Request headers</span></span>
|<span data-ttu-id="f3637-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3637-120">Header</span></span>|<span data-ttu-id="f3637-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f3637-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3637-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3637-122">Authorization</span></span>|<span data-ttu-id="f3637-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3637-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3637-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f3637-124">Accept</span></span>|<span data-ttu-id="f3637-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3637-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3637-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3637-126">Request body</span></span>
<span data-ttu-id="f3637-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3637-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="f3637-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span><span class="sxs-lookup"><span data-stu-id="f3637-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="f3637-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3637-129">Property</span></span>|<span data-ttu-id="f3637-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f3637-130">Type</span></span>|<span data-ttu-id="f3637-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f3637-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3637-132">id</span><span class="sxs-lookup"><span data-stu-id="f3637-132">id</span></span>|<span data-ttu-id="f3637-133">String</span><span class="sxs-lookup"><span data-stu-id="f3637-133">String</span></span>|<span data-ttu-id="f3637-134">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f3637-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="f3637-135">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="f3637-135">managedDeviceId</span></span>|<span data-ttu-id="f3637-136">String</span><span class="sxs-lookup"><span data-stu-id="f3637-136">String</span></span>|<span data-ttu-id="f3637-137">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f3637-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="f3637-138">процесснаме</span><span class="sxs-lookup"><span data-stu-id="f3637-138">processName</span></span>|<span data-ttu-id="f3637-139">String</span><span class="sxs-lookup"><span data-stu-id="f3637-139">String</span></span>|<span data-ttu-id="f3637-140">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f3637-140">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="f3637-141">productName</span><span class="sxs-lookup"><span data-stu-id="f3637-141">productName</span></span>|<span data-ttu-id="f3637-142">String</span><span class="sxs-lookup"><span data-stu-id="f3637-142">String</span></span>|<span data-ttu-id="f3637-143">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="f3637-143">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="f3637-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f3637-144">publisher</span></span>|<span data-ttu-id="f3637-145">String</span><span class="sxs-lookup"><span data-stu-id="f3637-145">String</span></span>|<span data-ttu-id="f3637-146">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="f3637-146">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="f3637-147">стартупимпактинмс</span><span class="sxs-lookup"><span data-stu-id="f3637-147">startupImpactInMs</span></span>|<span data-ttu-id="f3637-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f3637-148">Int32</span></span>|<span data-ttu-id="f3637-149">Влияние процесса запуска пользователя на устройство Analytics в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="f3637-149">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="f3637-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3637-150">Response</span></span>
<span data-ttu-id="f3637-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3637-151">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3637-152">Пример</span><span class="sxs-lookup"><span data-stu-id="f3637-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3637-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3637-153">Request</span></span>
<span data-ttu-id="f3637-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3637-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3637-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3637-155">Response</span></span>
<span data-ttu-id="f3637-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3637-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





