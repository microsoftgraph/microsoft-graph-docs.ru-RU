---
title: Обновление userExperienceAnalyticsImpactingProcess
description: Обновление свойств объекта userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2d1f2c3a2791e6536e701be35bc0c5c91e62949
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146225"
---
# <a name="update-userexperienceanalyticsimpactingprocess"></a><span data-ttu-id="1cf6b-103">Обновление userExperienceAnalyticsImpactingProcess</span><span class="sxs-lookup"><span data-stu-id="1cf6b-103">Update userExperienceAnalyticsImpactingProcess</span></span>

<span data-ttu-id="1cf6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cf6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cf6b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cf6b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cf6b-107">Обновление свойств объекта [userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6b-107">Update the properties of a [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cf6b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1cf6b-108">Prerequisites</span></span>
<span data-ttu-id="1cf6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cf6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cf6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cf6b-111">Permission type</span></span>|<span data-ttu-id="1cf6b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cf6b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cf6b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cf6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cf6b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cf6b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1cf6b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cf6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cf6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-116">Not supported.</span></span>|
|<span data-ttu-id="1cf6b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1cf6b-117">Application</span></span>|<span data-ttu-id="1cf6b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cf6b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cf6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cf6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="1cf6b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1cf6b-120">Request headers</span></span>
|<span data-ttu-id="1cf6b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cf6b-121">Header</span></span>|<span data-ttu-id="1cf6b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1cf6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cf6b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cf6b-123">Authorization</span></span>|<span data-ttu-id="1cf6b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cf6b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cf6b-125">Accept</span></span>|<span data-ttu-id="1cf6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cf6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cf6b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cf6b-127">Request body</span></span>
<span data-ttu-id="1cf6b-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6b-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

<span data-ttu-id="1cf6b-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="1cf6b-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).</span></span>

|<span data-ttu-id="1cf6b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cf6b-130">Property</span></span>|<span data-ttu-id="1cf6b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1cf6b-131">Type</span></span>|<span data-ttu-id="1cf6b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cf6b-133">id</span><span class="sxs-lookup"><span data-stu-id="1cf6b-133">id</span></span>|<span data-ttu-id="1cf6b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1cf6b-134">String</span></span>|<span data-ttu-id="1cf6b-135">Уникальный идентификатор объекта аналитики пользовательского интерфейса, который оказывает влияние на процесс.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-135">The unique identifier of the user experience analytics top impacting process entity.</span></span>|
|<span data-ttu-id="1cf6b-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="1cf6b-136">deviceId</span></span>|<span data-ttu-id="1cf6b-137">String</span><span class="sxs-lookup"><span data-stu-id="1cf6b-137">String</span></span>|<span data-ttu-id="1cf6b-138">Уникальный идентификатор влияемого устройства.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-138">The unique identifier of the impacted device.</span></span>|
|<span data-ttu-id="1cf6b-139">category</span><span class="sxs-lookup"><span data-stu-id="1cf6b-139">category</span></span>|<span data-ttu-id="1cf6b-140">String</span><span class="sxs-lookup"><span data-stu-id="1cf6b-140">String</span></span>|<span data-ttu-id="1cf6b-141">Категория воздействия процесса.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-141">The category of impacting process.</span></span>|
|<span data-ttu-id="1cf6b-142">processName</span><span class="sxs-lookup"><span data-stu-id="1cf6b-142">processName</span></span>|<span data-ttu-id="1cf6b-143">Строка</span><span class="sxs-lookup"><span data-stu-id="1cf6b-143">String</span></span>|<span data-ttu-id="1cf6b-144">Имя процесса.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-144">The process name.</span></span>|
|<span data-ttu-id="1cf6b-145">description</span><span class="sxs-lookup"><span data-stu-id="1cf6b-145">description</span></span>|<span data-ttu-id="1cf6b-146">Строка</span><span class="sxs-lookup"><span data-stu-id="1cf6b-146">String</span></span>|<span data-ttu-id="1cf6b-147">Описание процесса.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-147">The description of process.</span></span>|
|<span data-ttu-id="1cf6b-148">publisher</span><span class="sxs-lookup"><span data-stu-id="1cf6b-148">publisher</span></span>|<span data-ttu-id="1cf6b-149">String</span><span class="sxs-lookup"><span data-stu-id="1cf6b-149">String</span></span>|<span data-ttu-id="1cf6b-150">Издатель процесса.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-150">The publisher of the process.</span></span>|
|<span data-ttu-id="1cf6b-151">impactValue</span><span class="sxs-lookup"><span data-stu-id="1cf6b-151">impactValue</span></span>|<span data-ttu-id="1cf6b-152">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="1cf6b-152">Double</span></span>|<span data-ttu-id="1cf6b-153">Значение влияния процесса.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-153">The impact value of the process.</span></span> <span data-ttu-id="1cf6b-154">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="1cf6b-154">Valid values 0 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="1cf6b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cf6b-155">Response</span></span>
<span data-ttu-id="1cf6b-156">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-156">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cf6b-157">Пример</span><span class="sxs-lookup"><span data-stu-id="1cf6b-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cf6b-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cf6b-158">Request</span></span>
<span data-ttu-id="1cf6b-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```

### <a name="response"></a><span data-ttu-id="1cf6b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cf6b-160">Response</span></span>
<span data-ttu-id="1cf6b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cf6b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "faefd665-d665-faef-65d6-effa65d6effa",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```




