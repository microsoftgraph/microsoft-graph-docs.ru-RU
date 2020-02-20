---
title: Создание Усерекспериенцеаналитиксдевицестартуппроцесс
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуппроцесс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d48c58274e731afac219424bd333f840f9c37bf
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162010"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="94f30-103">Создание Усерекспериенцеаналитиксдевицестартуппроцесс</span><span class="sxs-lookup"><span data-stu-id="94f30-103">Create userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="94f30-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94f30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94f30-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94f30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94f30-106">Создание нового объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="94f30-106">Create a new [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94f30-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="94f30-107">Prerequisites</span></span>
<span data-ttu-id="94f30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94f30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94f30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94f30-110">Permission type</span></span>|<span data-ttu-id="94f30-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94f30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94f30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94f30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94f30-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f30-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="94f30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94f30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94f30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94f30-115">Not supported.</span></span>|
|<span data-ttu-id="94f30-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94f30-116">Application</span></span>|<span data-ttu-id="94f30-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f30-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94f30-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94f30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="94f30-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="94f30-119">Request headers</span></span>
|<span data-ttu-id="94f30-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94f30-120">Header</span></span>|<span data-ttu-id="94f30-121">Значение</span><span class="sxs-lookup"><span data-stu-id="94f30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94f30-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f30-122">Authorization</span></span>|<span data-ttu-id="94f30-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94f30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94f30-124">Accept</span><span class="sxs-lookup"><span data-stu-id="94f30-124">Accept</span></span>|<span data-ttu-id="94f30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94f30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94f30-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94f30-126">Request body</span></span>
<span data-ttu-id="94f30-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуппроцесс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94f30-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcess object.</span></span>

<span data-ttu-id="94f30-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуппроцесс.</span><span class="sxs-lookup"><span data-stu-id="94f30-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcess.</span></span>

|<span data-ttu-id="94f30-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="94f30-129">Property</span></span>|<span data-ttu-id="94f30-130">Тип</span><span class="sxs-lookup"><span data-stu-id="94f30-130">Type</span></span>|<span data-ttu-id="94f30-131">Описание</span><span class="sxs-lookup"><span data-stu-id="94f30-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f30-132">id</span><span class="sxs-lookup"><span data-stu-id="94f30-132">id</span></span>|<span data-ttu-id="94f30-133">String</span><span class="sxs-lookup"><span data-stu-id="94f30-133">String</span></span>|<span data-ttu-id="94f30-134">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="94f30-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="94f30-135">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="94f30-135">managedDeviceId</span></span>|<span data-ttu-id="94f30-136">String</span><span class="sxs-lookup"><span data-stu-id="94f30-136">String</span></span>|<span data-ttu-id="94f30-137">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="94f30-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="94f30-138">процесснаме</span><span class="sxs-lookup"><span data-stu-id="94f30-138">processName</span></span>|<span data-ttu-id="94f30-139">String</span><span class="sxs-lookup"><span data-stu-id="94f30-139">String</span></span>|<span data-ttu-id="94f30-140">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="94f30-140">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="94f30-141">productName</span><span class="sxs-lookup"><span data-stu-id="94f30-141">productName</span></span>|<span data-ttu-id="94f30-142">String</span><span class="sxs-lookup"><span data-stu-id="94f30-142">String</span></span>|<span data-ttu-id="94f30-143">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="94f30-143">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="94f30-144">publisher</span><span class="sxs-lookup"><span data-stu-id="94f30-144">publisher</span></span>|<span data-ttu-id="94f30-145">String</span><span class="sxs-lookup"><span data-stu-id="94f30-145">String</span></span>|<span data-ttu-id="94f30-146">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="94f30-146">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="94f30-147">стартупимпактинмс</span><span class="sxs-lookup"><span data-stu-id="94f30-147">startupImpactInMs</span></span>|<span data-ttu-id="94f30-148">Int32</span><span class="sxs-lookup"><span data-stu-id="94f30-148">Int32</span></span>|<span data-ttu-id="94f30-149">Влияние процесса запуска пользователя на устройство Analytics в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="94f30-149">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="94f30-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f30-150">Response</span></span>
<span data-ttu-id="94f30-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94f30-151">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94f30-152">Пример</span><span class="sxs-lookup"><span data-stu-id="94f30-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="94f30-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="94f30-153">Request</span></span>
<span data-ttu-id="94f30-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94f30-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94f30-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="94f30-155">Response</span></span>
<span data-ttu-id="94f30-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94f30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





