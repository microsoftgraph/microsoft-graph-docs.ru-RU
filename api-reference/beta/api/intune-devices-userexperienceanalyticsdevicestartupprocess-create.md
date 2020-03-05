---
title: Создание Усерекспериенцеаналитиксдевицестартуппроцесс
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуппроцесс.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7df6088f0d8af5bdb1dbdbe4303cd7a634b7522b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468336"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="15ff1-103">Создание Усерекспериенцеаналитиксдевицестартуппроцесс</span><span class="sxs-lookup"><span data-stu-id="15ff1-103">Create userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="15ff1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="15ff1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15ff1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15ff1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15ff1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15ff1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15ff1-107">Создание нового объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="15ff1-107">Create a new [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15ff1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15ff1-108">Prerequisites</span></span>
<span data-ttu-id="15ff1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ff1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15ff1-111">Permission type</span></span>|<span data-ttu-id="15ff1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15ff1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15ff1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15ff1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15ff1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ff1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="15ff1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15ff1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15ff1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15ff1-116">Not supported.</span></span>|
|<span data-ttu-id="15ff1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15ff1-117">Application</span></span>|<span data-ttu-id="15ff1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ff1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15ff1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15ff1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="15ff1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15ff1-120">Request headers</span></span>
|<span data-ttu-id="15ff1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15ff1-121">Header</span></span>|<span data-ttu-id="15ff1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15ff1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15ff1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15ff1-123">Authorization</span></span>|<span data-ttu-id="15ff1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15ff1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15ff1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15ff1-125">Accept</span></span>|<span data-ttu-id="15ff1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15ff1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15ff1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15ff1-127">Request body</span></span>
<span data-ttu-id="15ff1-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуппроцесс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15ff1-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcess object.</span></span>

<span data-ttu-id="15ff1-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуппроцесс.</span><span class="sxs-lookup"><span data-stu-id="15ff1-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcess.</span></span>

|<span data-ttu-id="15ff1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15ff1-130">Property</span></span>|<span data-ttu-id="15ff1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15ff1-131">Type</span></span>|<span data-ttu-id="15ff1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15ff1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ff1-133">id</span><span class="sxs-lookup"><span data-stu-id="15ff1-133">id</span></span>|<span data-ttu-id="15ff1-134">String</span><span class="sxs-lookup"><span data-stu-id="15ff1-134">String</span></span>|<span data-ttu-id="15ff1-135">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="15ff1-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="15ff1-136">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="15ff1-136">managedDeviceId</span></span>|<span data-ttu-id="15ff1-137">String</span><span class="sxs-lookup"><span data-stu-id="15ff1-137">String</span></span>|<span data-ttu-id="15ff1-138">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="15ff1-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="15ff1-139">процесснаме</span><span class="sxs-lookup"><span data-stu-id="15ff1-139">processName</span></span>|<span data-ttu-id="15ff1-140">String</span><span class="sxs-lookup"><span data-stu-id="15ff1-140">String</span></span>|<span data-ttu-id="15ff1-141">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="15ff1-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="15ff1-142">productName</span><span class="sxs-lookup"><span data-stu-id="15ff1-142">productName</span></span>|<span data-ttu-id="15ff1-143">String</span><span class="sxs-lookup"><span data-stu-id="15ff1-143">String</span></span>|<span data-ttu-id="15ff1-144">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="15ff1-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="15ff1-145">publisher</span><span class="sxs-lookup"><span data-stu-id="15ff1-145">publisher</span></span>|<span data-ttu-id="15ff1-146">String</span><span class="sxs-lookup"><span data-stu-id="15ff1-146">String</span></span>|<span data-ttu-id="15ff1-147">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="15ff1-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="15ff1-148">стартупимпактинмс</span><span class="sxs-lookup"><span data-stu-id="15ff1-148">startupImpactInMs</span></span>|<span data-ttu-id="15ff1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="15ff1-149">Int32</span></span>|<span data-ttu-id="15ff1-150">Влияние процесса запуска пользователя на устройство Analytics в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="15ff1-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="15ff1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="15ff1-151">Response</span></span>
<span data-ttu-id="15ff1-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15ff1-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15ff1-153">Пример</span><span class="sxs-lookup"><span data-stu-id="15ff1-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="15ff1-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="15ff1-154">Request</span></span>
<span data-ttu-id="15ff1-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15ff1-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15ff1-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="15ff1-156">Response</span></span>
<span data-ttu-id="15ff1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15ff1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





