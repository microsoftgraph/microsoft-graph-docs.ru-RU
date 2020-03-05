---
title: Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d7d85b0a3b94fa0969edcb85e8fb5d7f8a7eb23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468210"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="eaf28-103">Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце</span><span class="sxs-lookup"><span data-stu-id="eaf28-103">Update userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="eaf28-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eaf28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaf28-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaf28-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaf28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaf28-107">Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf28-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaf28-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eaf28-108">Prerequisites</span></span>
<span data-ttu-id="eaf28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf28-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf28-111">Permission type</span></span>|<span data-ttu-id="eaf28-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaf28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaf28-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaf28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaf28-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf28-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="eaf28-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaf28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaf28-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf28-116">Not supported.</span></span>|
|<span data-ttu-id="eaf28-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaf28-117">Application</span></span>|<span data-ttu-id="eaf28-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf28-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaf28-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaf28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="eaf28-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eaf28-120">Request headers</span></span>
|<span data-ttu-id="eaf28-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaf28-121">Header</span></span>|<span data-ttu-id="eaf28-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eaf28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaf28-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaf28-123">Authorization</span></span>|<span data-ttu-id="eaf28-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaf28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaf28-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eaf28-125">Accept</span></span>|<span data-ttu-id="eaf28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eaf28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf28-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eaf28-127">Request body</span></span>
<span data-ttu-id="eaf28-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaf28-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

<span data-ttu-id="eaf28-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span><span class="sxs-lookup"><span data-stu-id="eaf28-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span></span>

|<span data-ttu-id="eaf28-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaf28-130">Property</span></span>|<span data-ttu-id="eaf28-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eaf28-131">Type</span></span>|<span data-ttu-id="eaf28-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf28-133">id</span><span class="sxs-lookup"><span data-stu-id="eaf28-133">id</span></span>|<span data-ttu-id="eaf28-134">String</span><span class="sxs-lookup"><span data-stu-id="eaf28-134">String</span></span>|<span data-ttu-id="eaf28-135">Уникальный идентификатор производительности процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="eaf28-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="eaf28-136">процесснаме</span><span class="sxs-lookup"><span data-stu-id="eaf28-136">processName</span></span>|<span data-ttu-id="eaf28-137">String</span><span class="sxs-lookup"><span data-stu-id="eaf28-137">String</span></span>|<span data-ttu-id="eaf28-138">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="eaf28-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="eaf28-139">productName</span><span class="sxs-lookup"><span data-stu-id="eaf28-139">productName</span></span>|<span data-ttu-id="eaf28-140">String</span><span class="sxs-lookup"><span data-stu-id="eaf28-140">String</span></span>|<span data-ttu-id="eaf28-141">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="eaf28-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="eaf28-142">publisher</span><span class="sxs-lookup"><span data-stu-id="eaf28-142">publisher</span></span>|<span data-ttu-id="eaf28-143">String</span><span class="sxs-lookup"><span data-stu-id="eaf28-143">String</span></span>|<span data-ttu-id="eaf28-144">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="eaf28-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="eaf28-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="eaf28-145">deviceCount</span></span>|<span data-ttu-id="eaf28-146">Int64</span><span class="sxs-lookup"><span data-stu-id="eaf28-146">Int64</span></span>|<span data-ttu-id="eaf28-147">Сводка по процессу запуска при запуске устройства с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="eaf28-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="eaf28-148">медианимпактинмс</span><span class="sxs-lookup"><span data-stu-id="eaf28-148">medianImpactInMs</span></span>|<span data-ttu-id="eaf28-149">Int32</span><span class="sxs-lookup"><span data-stu-id="eaf28-149">Int32</span></span>|<span data-ttu-id="eaf28-150">Поведение при запуске устройства Analytics для пользователя в течение среднего влияния в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="eaf28-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="eaf28-151">тоталимпактинмс</span><span class="sxs-lookup"><span data-stu-id="eaf28-151">totalImpactInMs</span></span>|<span data-ttu-id="eaf28-152">Int32</span><span class="sxs-lookup"><span data-stu-id="eaf28-152">Int32</span></span>|<span data-ttu-id="eaf28-153">Общее влияние на процесс запуска пользователя при запуске устройства Analytics (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="eaf28-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="eaf28-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaf28-154">Response</span></span>
<span data-ttu-id="eaf28-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eaf28-155">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaf28-156">Пример</span><span class="sxs-lookup"><span data-stu-id="eaf28-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaf28-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaf28-157">Request</span></span>
<span data-ttu-id="eaf28-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaf28-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```

### <a name="response"></a><span data-ttu-id="eaf28-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaf28-159">Response</span></span>
<span data-ttu-id="eaf28-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaf28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "86c4355c-355c-86c4-5c35-c4865c35c486",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```





