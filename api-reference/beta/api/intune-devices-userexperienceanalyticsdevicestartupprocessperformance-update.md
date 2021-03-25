---
title: Обновление userExperienceAnalyticsDeviceStartupProcessPerformance
description: Обновление свойств объекта userExperienceAnalyticsDeviceStartupProcessPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d613306a9630b1ed7900ab05c7daa67b43c28ca2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157928"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="157a9-103">Обновление userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="157a9-103">Update userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="157a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="157a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="157a9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="157a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="157a9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="157a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="157a9-107">Обновление свойств объекта [userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)</span><span class="sxs-lookup"><span data-stu-id="157a9-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="157a9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="157a9-108">Prerequisites</span></span>
<span data-ttu-id="157a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="157a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="157a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="157a9-111">Permission type</span></span>|<span data-ttu-id="157a9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="157a9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="157a9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="157a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="157a9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157a9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="157a9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="157a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="157a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="157a9-116">Not supported.</span></span>|
|<span data-ttu-id="157a9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="157a9-117">Application</span></span>|<span data-ttu-id="157a9-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="157a9-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="157a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="157a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="157a9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="157a9-120">Request headers</span></span>
|<span data-ttu-id="157a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="157a9-121">Header</span></span>|<span data-ttu-id="157a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="157a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="157a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="157a9-123">Authorization</span></span>|<span data-ttu-id="157a9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="157a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="157a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="157a9-125">Accept</span></span>|<span data-ttu-id="157a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="157a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="157a9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="157a9-127">Request body</span></span>
<span data-ttu-id="157a9-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)</span><span class="sxs-lookup"><span data-stu-id="157a9-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

<span data-ttu-id="157a9-129">В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)</span><span class="sxs-lookup"><span data-stu-id="157a9-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span></span>

|<span data-ttu-id="157a9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="157a9-130">Property</span></span>|<span data-ttu-id="157a9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="157a9-131">Type</span></span>|<span data-ttu-id="157a9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="157a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="157a9-133">id</span><span class="sxs-lookup"><span data-stu-id="157a9-133">id</span></span>|<span data-ttu-id="157a9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="157a9-134">String</span></span>|<span data-ttu-id="157a9-135">Уникальный идентификатор производительности процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="157a9-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="157a9-136">processName</span><span class="sxs-lookup"><span data-stu-id="157a9-136">processName</span></span>|<span data-ttu-id="157a9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="157a9-137">String</span></span>|<span data-ttu-id="157a9-138">Имя процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="157a9-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="157a9-139">productName</span><span class="sxs-lookup"><span data-stu-id="157a9-139">productName</span></span>|<span data-ttu-id="157a9-140">String</span><span class="sxs-lookup"><span data-stu-id="157a9-140">String</span></span>|<span data-ttu-id="157a9-141">Имя продукта процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="157a9-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="157a9-142">publisher</span><span class="sxs-lookup"><span data-stu-id="157a9-142">publisher</span></span>|<span data-ttu-id="157a9-143">String</span><span class="sxs-lookup"><span data-stu-id="157a9-143">String</span></span>|<span data-ttu-id="157a9-144">Издатель процесса запуска устройства для аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="157a9-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="157a9-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="157a9-145">deviceCount</span></span>|<span data-ttu-id="157a9-146">Int64</span><span class="sxs-lookup"><span data-stu-id="157a9-146">Int64</span></span>|<span data-ttu-id="157a9-147">Процесс запуска устройства аналитики пользовательских интерфейсов суммирован.</span><span class="sxs-lookup"><span data-stu-id="157a9-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="157a9-148">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="157a9-148">medianImpactInMs</span></span>|<span data-ttu-id="157a9-149">Int32</span><span class="sxs-lookup"><span data-stu-id="157a9-149">Int32</span></span>|<span data-ttu-id="157a9-150">Медиана процесса запуска устройств для аналитики пользовательских интерфейсов в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="157a9-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="157a9-151">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="157a9-151">totalImpactInMs</span></span>|<span data-ttu-id="157a9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="157a9-152">Int32</span></span>|<span data-ttu-id="157a9-153">Процесс запуска устройства для аналитики пользовательских интерфейсов полностью влияет на миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="157a9-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="157a9-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="157a9-154">Response</span></span>
<span data-ttu-id="157a9-155">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="157a9-155">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="157a9-156">Пример</span><span class="sxs-lookup"><span data-stu-id="157a9-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="157a9-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="157a9-157">Request</span></span>
<span data-ttu-id="157a9-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="157a9-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="157a9-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="157a9-159">Response</span></span>
<span data-ttu-id="157a9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="157a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




