---
title: Создание Усерекспериенцеаналитиксдевицестартуппроцесс
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуппроцесс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b7c9e1eca9c70e65b1844071d22650a8de33c28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082569"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="28d2f-103">Создание Усерекспериенцеаналитиксдевицестартуппроцесс</span><span class="sxs-lookup"><span data-stu-id="28d2f-103">Create userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="28d2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28d2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28d2f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28d2f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28d2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28d2f-107">Создание нового объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="28d2f-107">Create a new [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28d2f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28d2f-108">Prerequisites</span></span>
<span data-ttu-id="28d2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28d2f-111">Permission type</span></span>|<span data-ttu-id="28d2f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28d2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28d2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28d2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28d2f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d2f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="28d2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28d2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28d2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d2f-116">Not supported.</span></span>|
|<span data-ttu-id="28d2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28d2f-117">Application</span></span>|<span data-ttu-id="28d2f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d2f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28d2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28d2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="28d2f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28d2f-120">Request headers</span></span>
|<span data-ttu-id="28d2f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28d2f-121">Header</span></span>|<span data-ttu-id="28d2f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28d2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28d2f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28d2f-123">Authorization</span></span>|<span data-ttu-id="28d2f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28d2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28d2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28d2f-125">Accept</span></span>|<span data-ttu-id="28d2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28d2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28d2f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28d2f-127">Request body</span></span>
<span data-ttu-id="28d2f-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуппроцесс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28d2f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcess object.</span></span>

<span data-ttu-id="28d2f-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуппроцесс.</span><span class="sxs-lookup"><span data-stu-id="28d2f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcess.</span></span>

|<span data-ttu-id="28d2f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28d2f-130">Property</span></span>|<span data-ttu-id="28d2f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28d2f-131">Type</span></span>|<span data-ttu-id="28d2f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28d2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28d2f-133">id</span><span class="sxs-lookup"><span data-stu-id="28d2f-133">id</span></span>|<span data-ttu-id="28d2f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="28d2f-134">String</span></span>|<span data-ttu-id="28d2f-135">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="28d2f-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="28d2f-136">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="28d2f-136">managedDeviceId</span></span>|<span data-ttu-id="28d2f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="28d2f-137">String</span></span>|<span data-ttu-id="28d2f-138">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="28d2f-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="28d2f-139">процесснаме</span><span class="sxs-lookup"><span data-stu-id="28d2f-139">processName</span></span>|<span data-ttu-id="28d2f-140">Строка</span><span class="sxs-lookup"><span data-stu-id="28d2f-140">String</span></span>|<span data-ttu-id="28d2f-141">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="28d2f-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="28d2f-142">productName</span><span class="sxs-lookup"><span data-stu-id="28d2f-142">productName</span></span>|<span data-ttu-id="28d2f-143">String</span><span class="sxs-lookup"><span data-stu-id="28d2f-143">String</span></span>|<span data-ttu-id="28d2f-144">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="28d2f-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="28d2f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="28d2f-145">publisher</span></span>|<span data-ttu-id="28d2f-146">String</span><span class="sxs-lookup"><span data-stu-id="28d2f-146">String</span></span>|<span data-ttu-id="28d2f-147">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="28d2f-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="28d2f-148">стартупимпактинмс</span><span class="sxs-lookup"><span data-stu-id="28d2f-148">startupImpactInMs</span></span>|<span data-ttu-id="28d2f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="28d2f-149">Int32</span></span>|<span data-ttu-id="28d2f-150">Влияние процесса запуска пользователя на устройство Analytics в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="28d2f-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="28d2f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d2f-151">Response</span></span>
<span data-ttu-id="28d2f-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28d2f-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d2f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="28d2f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="28d2f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="28d2f-154">Request</span></span>
<span data-ttu-id="28d2f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28d2f-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="28d2f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d2f-156">Response</span></span>
<span data-ttu-id="28d2f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28d2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






