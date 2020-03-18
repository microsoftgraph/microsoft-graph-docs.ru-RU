---
title: Создание Усерекспериенцеаналитиксдевицестартуппроцесс
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуппроцесс.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e81e4066e280070e3b520ef08bd7728dcca020bd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813918"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="009fd-103">Создание Усерекспериенцеаналитиксдевицестартуппроцесс</span><span class="sxs-lookup"><span data-stu-id="009fd-103">Create userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="009fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="009fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="009fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="009fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="009fd-106">Создание нового объекта [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) .</span><span class="sxs-lookup"><span data-stu-id="009fd-106">Create a new [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="009fd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="009fd-107">Prerequisites</span></span>
<span data-ttu-id="009fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="009fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="009fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="009fd-110">Permission type</span></span>|<span data-ttu-id="009fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="009fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="009fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="009fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="009fd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="009fd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="009fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="009fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="009fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="009fd-115">Not supported.</span></span>|
|<span data-ttu-id="009fd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="009fd-116">Application</span></span>|<span data-ttu-id="009fd-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="009fd-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="009fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="009fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="009fd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="009fd-119">Request headers</span></span>
|<span data-ttu-id="009fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="009fd-120">Header</span></span>|<span data-ttu-id="009fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="009fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="009fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="009fd-122">Authorization</span></span>|<span data-ttu-id="009fd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="009fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="009fd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="009fd-124">Accept</span></span>|<span data-ttu-id="009fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="009fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="009fd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="009fd-126">Request body</span></span>
<span data-ttu-id="009fd-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуппроцесс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="009fd-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcess object.</span></span>

<span data-ttu-id="009fd-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуппроцесс.</span><span class="sxs-lookup"><span data-stu-id="009fd-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcess.</span></span>

|<span data-ttu-id="009fd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="009fd-129">Property</span></span>|<span data-ttu-id="009fd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="009fd-130">Type</span></span>|<span data-ttu-id="009fd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="009fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="009fd-132">id</span><span class="sxs-lookup"><span data-stu-id="009fd-132">id</span></span>|<span data-ttu-id="009fd-133">String</span><span class="sxs-lookup"><span data-stu-id="009fd-133">String</span></span>|<span data-ttu-id="009fd-134">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="009fd-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="009fd-135">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="009fd-135">managedDeviceId</span></span>|<span data-ttu-id="009fd-136">String</span><span class="sxs-lookup"><span data-stu-id="009fd-136">String</span></span>|<span data-ttu-id="009fd-137">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="009fd-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="009fd-138">процесснаме</span><span class="sxs-lookup"><span data-stu-id="009fd-138">processName</span></span>|<span data-ttu-id="009fd-139">String</span><span class="sxs-lookup"><span data-stu-id="009fd-139">String</span></span>|<span data-ttu-id="009fd-140">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="009fd-140">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="009fd-141">productName</span><span class="sxs-lookup"><span data-stu-id="009fd-141">productName</span></span>|<span data-ttu-id="009fd-142">String</span><span class="sxs-lookup"><span data-stu-id="009fd-142">String</span></span>|<span data-ttu-id="009fd-143">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="009fd-143">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="009fd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="009fd-144">publisher</span></span>|<span data-ttu-id="009fd-145">String</span><span class="sxs-lookup"><span data-stu-id="009fd-145">String</span></span>|<span data-ttu-id="009fd-146">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="009fd-146">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="009fd-147">стартупимпактинмс</span><span class="sxs-lookup"><span data-stu-id="009fd-147">startupImpactInMs</span></span>|<span data-ttu-id="009fd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="009fd-148">Int32</span></span>|<span data-ttu-id="009fd-149">Влияние процесса запуска пользователя на устройство Analytics в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="009fd-149">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="009fd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="009fd-150">Response</span></span>
<span data-ttu-id="009fd-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуппроцесс](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="009fd-151">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="009fd-152">Пример</span><span class="sxs-lookup"><span data-stu-id="009fd-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="009fd-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="009fd-153">Request</span></span>
<span data-ttu-id="009fd-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="009fd-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="009fd-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="009fd-155">Response</span></span>
<span data-ttu-id="009fd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="009fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




