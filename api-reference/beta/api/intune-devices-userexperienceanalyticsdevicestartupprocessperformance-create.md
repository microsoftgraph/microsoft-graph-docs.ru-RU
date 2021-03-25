---
title: Создание userExperienceAnalyticsDeviceStartupProcessPerformance
description: Создание нового объекта userExperienceAnalyticsDeviceStartupProcessPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5da588641c970adf10d3631f232669743d011c2d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154030"
---
# <a name="create-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="fdc18-103">Создание userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="fdc18-103">Create userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="fdc18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdc18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdc18-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdc18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdc18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc18-107">Создание нового [объекта userExperienceAnalyticsDeviceStartupProcessPerformance.](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)</span><span class="sxs-lookup"><span data-stu-id="fdc18-107">Create a new [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdc18-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fdc18-108">Prerequisites</span></span>
<span data-ttu-id="fdc18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdc18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdc18-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdc18-111">Permission type</span></span>|<span data-ttu-id="fdc18-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdc18-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdc18-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdc18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdc18-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdc18-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fdc18-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdc18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdc18-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc18-116">Not supported.</span></span>|
|<span data-ttu-id="fdc18-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fdc18-117">Application</span></span>|<span data-ttu-id="fdc18-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdc18-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdc18-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdc18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="fdc18-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fdc18-120">Request headers</span></span>
|<span data-ttu-id="fdc18-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdc18-121">Header</span></span>|<span data-ttu-id="fdc18-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fdc18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdc18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdc18-123">Authorization</span></span>|<span data-ttu-id="fdc18-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdc18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdc18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fdc18-125">Accept</span></span>|<span data-ttu-id="fdc18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdc18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdc18-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdc18-127">Request body</span></span>
<span data-ttu-id="fdc18-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsDeviceStartupProcessPerformance.</span><span class="sxs-lookup"><span data-stu-id="fdc18-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcessPerformance object.</span></span>

<span data-ttu-id="fdc18-129">В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsDeviceStartupProcessPerformance.</span><span class="sxs-lookup"><span data-stu-id="fdc18-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcessPerformance.</span></span>

|<span data-ttu-id="fdc18-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdc18-130">Property</span></span>|<span data-ttu-id="fdc18-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fdc18-131">Type</span></span>|<span data-ttu-id="fdc18-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc18-133">id</span><span class="sxs-lookup"><span data-stu-id="fdc18-133">id</span></span>|<span data-ttu-id="fdc18-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fdc18-134">String</span></span>|<span data-ttu-id="fdc18-135">Уникальный идентификатор производительности процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="fdc18-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="fdc18-136">processName</span><span class="sxs-lookup"><span data-stu-id="fdc18-136">processName</span></span>|<span data-ttu-id="fdc18-137">Строка</span><span class="sxs-lookup"><span data-stu-id="fdc18-137">String</span></span>|<span data-ttu-id="fdc18-138">Имя процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="fdc18-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="fdc18-139">productName</span><span class="sxs-lookup"><span data-stu-id="fdc18-139">productName</span></span>|<span data-ttu-id="fdc18-140">String</span><span class="sxs-lookup"><span data-stu-id="fdc18-140">String</span></span>|<span data-ttu-id="fdc18-141">Имя продукта процесса запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="fdc18-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="fdc18-142">publisher</span><span class="sxs-lookup"><span data-stu-id="fdc18-142">publisher</span></span>|<span data-ttu-id="fdc18-143">String</span><span class="sxs-lookup"><span data-stu-id="fdc18-143">String</span></span>|<span data-ttu-id="fdc18-144">Издатель процесса запуска устройства для аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="fdc18-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="fdc18-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="fdc18-145">deviceCount</span></span>|<span data-ttu-id="fdc18-146">Int64</span><span class="sxs-lookup"><span data-stu-id="fdc18-146">Int64</span></span>|<span data-ttu-id="fdc18-147">Процесс запуска устройства аналитики пользовательских интерфейсов суммирован.</span><span class="sxs-lookup"><span data-stu-id="fdc18-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="fdc18-148">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="fdc18-148">medianImpactInMs</span></span>|<span data-ttu-id="fdc18-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fdc18-149">Int32</span></span>|<span data-ttu-id="fdc18-150">Медиана процесса запуска устройств для аналитики пользовательских интерфейсов в миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="fdc18-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="fdc18-151">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="fdc18-151">totalImpactInMs</span></span>|<span data-ttu-id="fdc18-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fdc18-152">Int32</span></span>|<span data-ttu-id="fdc18-153">Процесс запуска устройства для аналитики пользовательских интерфейсов полностью влияет на миллисекунд.</span><span class="sxs-lookup"><span data-stu-id="fdc18-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="fdc18-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdc18-154">Response</span></span>
<span data-ttu-id="fdc18-155">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fdc18-155">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdc18-156">Пример</span><span class="sxs-lookup"><span data-stu-id="fdc18-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdc18-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdc18-157">Request</span></span>
<span data-ttu-id="fdc18-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdc18-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
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

### <a name="response"></a><span data-ttu-id="fdc18-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdc18-159">Response</span></span>
<span data-ttu-id="fdc18-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdc18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




