---
title: Обновление userExperienceAnalyticsImpactingProcess
description: Обновление свойств объекта userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18be2d4556c454d387418a0ba434aa51bc0ea7e3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446750"
---
# <a name="update-userexperienceanalyticsimpactingprocess"></a><span data-ttu-id="0de91-103">Обновление userExperienceAnalyticsImpactingProcess</span><span class="sxs-lookup"><span data-stu-id="0de91-103">Update userExperienceAnalyticsImpactingProcess</span></span>

<span data-ttu-id="0de91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0de91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0de91-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0de91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0de91-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0de91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0de91-107">Обновление свойств объекта [userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="0de91-107">Update the properties of a [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0de91-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0de91-108">Prerequisites</span></span>
<span data-ttu-id="0de91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0de91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0de91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0de91-111">Permission type</span></span>|<span data-ttu-id="0de91-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0de91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0de91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0de91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0de91-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0de91-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0de91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0de91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0de91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0de91-116">Not supported.</span></span>|
|<span data-ttu-id="0de91-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0de91-117">Application</span></span>|<span data-ttu-id="0de91-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0de91-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0de91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0de91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="0de91-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0de91-120">Request headers</span></span>
|<span data-ttu-id="0de91-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0de91-121">Header</span></span>|<span data-ttu-id="0de91-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0de91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0de91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0de91-123">Authorization</span></span>|<span data-ttu-id="0de91-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0de91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0de91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0de91-125">Accept</span></span>|<span data-ttu-id="0de91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0de91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0de91-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0de91-127">Request body</span></span>
<span data-ttu-id="0de91-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="0de91-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

<span data-ttu-id="0de91-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="0de91-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).</span></span>

|<span data-ttu-id="0de91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0de91-130">Property</span></span>|<span data-ttu-id="0de91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0de91-131">Type</span></span>|<span data-ttu-id="0de91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0de91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0de91-133">id</span><span class="sxs-lookup"><span data-stu-id="0de91-133">id</span></span>|<span data-ttu-id="0de91-134">String</span><span class="sxs-lookup"><span data-stu-id="0de91-134">String</span></span>|<span data-ttu-id="0de91-135">Уникальный идентификатор объекта аналитики пользовательского интерфейса, который оказывает влияние на процесс.</span><span class="sxs-lookup"><span data-stu-id="0de91-135">The unique identifier of the user experience analytics top impacting process entity.</span></span>|
|<span data-ttu-id="0de91-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="0de91-136">deviceId</span></span>|<span data-ttu-id="0de91-137">String</span><span class="sxs-lookup"><span data-stu-id="0de91-137">String</span></span>|<span data-ttu-id="0de91-138">Уникальный идентификатор влияемого устройства.</span><span class="sxs-lookup"><span data-stu-id="0de91-138">The unique identifier of the impacted device.</span></span>|
|<span data-ttu-id="0de91-139">category</span><span class="sxs-lookup"><span data-stu-id="0de91-139">category</span></span>|<span data-ttu-id="0de91-140">String</span><span class="sxs-lookup"><span data-stu-id="0de91-140">String</span></span>|<span data-ttu-id="0de91-141">Категория воздействия процесса.</span><span class="sxs-lookup"><span data-stu-id="0de91-141">The category of impacting process.</span></span>|
|<span data-ttu-id="0de91-142">processName</span><span class="sxs-lookup"><span data-stu-id="0de91-142">processName</span></span>|<span data-ttu-id="0de91-143">String</span><span class="sxs-lookup"><span data-stu-id="0de91-143">String</span></span>|<span data-ttu-id="0de91-144">Имя процесса.</span><span class="sxs-lookup"><span data-stu-id="0de91-144">The process name.</span></span>|
|<span data-ttu-id="0de91-145">description</span><span class="sxs-lookup"><span data-stu-id="0de91-145">description</span></span>|<span data-ttu-id="0de91-146">String</span><span class="sxs-lookup"><span data-stu-id="0de91-146">String</span></span>|<span data-ttu-id="0de91-147">Описание процесса.</span><span class="sxs-lookup"><span data-stu-id="0de91-147">The description of process.</span></span>|
|<span data-ttu-id="0de91-148">publisher</span><span class="sxs-lookup"><span data-stu-id="0de91-148">publisher</span></span>|<span data-ttu-id="0de91-149">String</span><span class="sxs-lookup"><span data-stu-id="0de91-149">String</span></span>|<span data-ttu-id="0de91-150">Издатель процесса.</span><span class="sxs-lookup"><span data-stu-id="0de91-150">The publisher of the process.</span></span>|
|<span data-ttu-id="0de91-151">impactValue</span><span class="sxs-lookup"><span data-stu-id="0de91-151">impactValue</span></span>|<span data-ttu-id="0de91-152">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0de91-152">Double</span></span>|<span data-ttu-id="0de91-153">Значение влияния процесса.</span><span class="sxs-lookup"><span data-stu-id="0de91-153">The impact value of the process.</span></span> <span data-ttu-id="0de91-154">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="0de91-154">Valid values 0 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="0de91-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0de91-155">Response</span></span>
<span data-ttu-id="0de91-156">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0de91-156">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0de91-157">Пример</span><span class="sxs-lookup"><span data-stu-id="0de91-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0de91-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0de91-158">Request</span></span>
<span data-ttu-id="0de91-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0de91-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0de91-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0de91-160">Response</span></span>
<span data-ttu-id="0de91-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0de91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




