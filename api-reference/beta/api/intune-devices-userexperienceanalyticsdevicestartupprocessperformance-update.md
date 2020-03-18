---
title: Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6af5f340e0751eb0528e57172b1afef2163916eb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813854"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="4c6ca-103">Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце</span><span class="sxs-lookup"><span data-stu-id="4c6ca-103">Update userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

> <span data-ttu-id="4c6ca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c6ca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c6ca-106">Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="4c6ca-106">Update the properties of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c6ca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4c6ca-107">Prerequisites</span></span>
<span data-ttu-id="4c6ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c6ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c6ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c6ca-110">Permission type</span></span>|<span data-ttu-id="4c6ca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c6ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c6ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c6ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c6ca-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c6ca-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4c6ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c6ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c6ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-115">Not supported.</span></span>|
|<span data-ttu-id="4c6ca-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4c6ca-116">Application</span></span>|<span data-ttu-id="4c6ca-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c6ca-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c6ca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c6ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="4c6ca-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c6ca-119">Request headers</span></span>
|<span data-ttu-id="4c6ca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c6ca-120">Header</span></span>|<span data-ttu-id="4c6ca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4c6ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c6ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c6ca-122">Authorization</span></span>|<span data-ttu-id="4c6ca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c6ca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4c6ca-124">Accept</span></span>|<span data-ttu-id="4c6ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c6ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c6ca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c6ca-126">Request body</span></span>
<span data-ttu-id="4c6ca-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

<span data-ttu-id="4c6ca-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span><span class="sxs-lookup"><span data-stu-id="4c6ca-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span></span>

|<span data-ttu-id="4c6ca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c6ca-129">Property</span></span>|<span data-ttu-id="4c6ca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4c6ca-130">Type</span></span>|<span data-ttu-id="4c6ca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4c6ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c6ca-132">id</span><span class="sxs-lookup"><span data-stu-id="4c6ca-132">id</span></span>|<span data-ttu-id="4c6ca-133">String</span><span class="sxs-lookup"><span data-stu-id="4c6ca-133">String</span></span>|<span data-ttu-id="4c6ca-134">Уникальный идентификатор производительности процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-134">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="4c6ca-135">процесснаме</span><span class="sxs-lookup"><span data-stu-id="4c6ca-135">processName</span></span>|<span data-ttu-id="4c6ca-136">String</span><span class="sxs-lookup"><span data-stu-id="4c6ca-136">String</span></span>|<span data-ttu-id="4c6ca-137">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-137">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="4c6ca-138">productName</span><span class="sxs-lookup"><span data-stu-id="4c6ca-138">productName</span></span>|<span data-ttu-id="4c6ca-139">String</span><span class="sxs-lookup"><span data-stu-id="4c6ca-139">String</span></span>|<span data-ttu-id="4c6ca-140">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="4c6ca-140">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="4c6ca-141">publisher</span><span class="sxs-lookup"><span data-stu-id="4c6ca-141">publisher</span></span>|<span data-ttu-id="4c6ca-142">String</span><span class="sxs-lookup"><span data-stu-id="4c6ca-142">String</span></span>|<span data-ttu-id="4c6ca-143">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-143">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="4c6ca-144">deviceCount</span><span class="sxs-lookup"><span data-stu-id="4c6ca-144">deviceCount</span></span>|<span data-ttu-id="4c6ca-145">Int64</span><span class="sxs-lookup"><span data-stu-id="4c6ca-145">Int64</span></span>|<span data-ttu-id="4c6ca-146">Сводка по процессу запуска при запуске устройства с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-146">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="4c6ca-147">медианимпактинмс</span><span class="sxs-lookup"><span data-stu-id="4c6ca-147">medianImpactInMs</span></span>|<span data-ttu-id="4c6ca-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4c6ca-148">Int32</span></span>|<span data-ttu-id="4c6ca-149">Поведение при запуске устройства Analytics для пользователя в течение среднего влияния в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-149">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="4c6ca-150">тоталимпактинмс</span><span class="sxs-lookup"><span data-stu-id="4c6ca-150">totalImpactInMs</span></span>|<span data-ttu-id="4c6ca-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4c6ca-151">Int32</span></span>|<span data-ttu-id="4c6ca-152">Общее влияние на процесс запуска пользователя при запуске устройства Analytics (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="4c6ca-152">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="4c6ca-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c6ca-153">Response</span></span>
<span data-ttu-id="4c6ca-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-154">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c6ca-155">Пример</span><span class="sxs-lookup"><span data-stu-id="4c6ca-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c6ca-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c6ca-156">Request</span></span>
<span data-ttu-id="4c6ca-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c6ca-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c6ca-158">Response</span></span>
<span data-ttu-id="4c6ca-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c6ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




