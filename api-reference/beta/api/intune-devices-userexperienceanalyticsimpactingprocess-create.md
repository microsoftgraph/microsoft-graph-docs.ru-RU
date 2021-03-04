---
title: Создание userExperienceAnalyticsImpactingProcess
description: Создание нового объекта userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7c1122e05a574438d1df09c1fe1ae4fa853fb75
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447450"
---
# <a name="create-userexperienceanalyticsimpactingprocess"></a><span data-ttu-id="0a8ad-103">Создание userExperienceAnalyticsImpactingProcess</span><span class="sxs-lookup"><span data-stu-id="0a8ad-103">Create userExperienceAnalyticsImpactingProcess</span></span>

<span data-ttu-id="0a8ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a8ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a8ad-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a8ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a8ad-107">Создание нового [объекта userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)</span><span class="sxs-lookup"><span data-stu-id="0a8ad-107">Create a new [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a8ad-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a8ad-108">Prerequisites</span></span>
<span data-ttu-id="0a8ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a8ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a8ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a8ad-111">Permission type</span></span>|<span data-ttu-id="0a8ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a8ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a8ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a8ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a8ad-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a8ad-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0a8ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a8ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a8ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-116">Not supported.</span></span>|
|<span data-ttu-id="0a8ad-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a8ad-117">Application</span></span>|<span data-ttu-id="0a8ad-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a8ad-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a8ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a8ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsImpactingProcess
```

## <a name="request-headers"></a><span data-ttu-id="0a8ad-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a8ad-120">Request headers</span></span>
|<span data-ttu-id="0a8ad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a8ad-121">Header</span></span>|<span data-ttu-id="0a8ad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a8ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a8ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a8ad-123">Authorization</span></span>|<span data-ttu-id="0a8ad-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a8ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a8ad-125">Accept</span></span>|<span data-ttu-id="0a8ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a8ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a8ad-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a8ad-127">Request body</span></span>
<span data-ttu-id="0a8ad-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsImpactingProcess.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-128">In the request body, supply a JSON representation for the userExperienceAnalyticsImpactingProcess object.</span></span>

<span data-ttu-id="0a8ad-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsImpactingProcess.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-129">The following table shows the properties that are required when you create the userExperienceAnalyticsImpactingProcess.</span></span>

|<span data-ttu-id="0a8ad-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a8ad-130">Property</span></span>|<span data-ttu-id="0a8ad-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a8ad-131">Type</span></span>|<span data-ttu-id="0a8ad-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a8ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a8ad-133">id</span><span class="sxs-lookup"><span data-stu-id="0a8ad-133">id</span></span>|<span data-ttu-id="0a8ad-134">String</span><span class="sxs-lookup"><span data-stu-id="0a8ad-134">String</span></span>|<span data-ttu-id="0a8ad-135">Уникальный идентификатор объекта аналитики пользовательского интерфейса, который оказывает влияние на процесс.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-135">The unique identifier of the user experience analytics top impacting process entity.</span></span>|
|<span data-ttu-id="0a8ad-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="0a8ad-136">deviceId</span></span>|<span data-ttu-id="0a8ad-137">String</span><span class="sxs-lookup"><span data-stu-id="0a8ad-137">String</span></span>|<span data-ttu-id="0a8ad-138">Уникальный идентификатор влияемого устройства.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-138">The unique identifier of the impacted device.</span></span>|
|<span data-ttu-id="0a8ad-139">category</span><span class="sxs-lookup"><span data-stu-id="0a8ad-139">category</span></span>|<span data-ttu-id="0a8ad-140">String</span><span class="sxs-lookup"><span data-stu-id="0a8ad-140">String</span></span>|<span data-ttu-id="0a8ad-141">Категория воздействия процесса.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-141">The category of impacting process.</span></span>|
|<span data-ttu-id="0a8ad-142">processName</span><span class="sxs-lookup"><span data-stu-id="0a8ad-142">processName</span></span>|<span data-ttu-id="0a8ad-143">String</span><span class="sxs-lookup"><span data-stu-id="0a8ad-143">String</span></span>|<span data-ttu-id="0a8ad-144">Имя процесса.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-144">The process name.</span></span>|
|<span data-ttu-id="0a8ad-145">description</span><span class="sxs-lookup"><span data-stu-id="0a8ad-145">description</span></span>|<span data-ttu-id="0a8ad-146">String</span><span class="sxs-lookup"><span data-stu-id="0a8ad-146">String</span></span>|<span data-ttu-id="0a8ad-147">Описание процесса.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-147">The description of process.</span></span>|
|<span data-ttu-id="0a8ad-148">publisher</span><span class="sxs-lookup"><span data-stu-id="0a8ad-148">publisher</span></span>|<span data-ttu-id="0a8ad-149">String</span><span class="sxs-lookup"><span data-stu-id="0a8ad-149">String</span></span>|<span data-ttu-id="0a8ad-150">Издатель процесса.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-150">The publisher of the process.</span></span>|
|<span data-ttu-id="0a8ad-151">impactValue</span><span class="sxs-lookup"><span data-stu-id="0a8ad-151">impactValue</span></span>|<span data-ttu-id="0a8ad-152">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0a8ad-152">Double</span></span>|<span data-ttu-id="0a8ad-153">Значение влияния процесса.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-153">The impact value of the process.</span></span> <span data-ttu-id="0a8ad-154">Допустимые значения от 0 до 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="0a8ad-154">Valid values 0 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="0a8ad-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a8ad-155">Response</span></span>
<span data-ttu-id="0a8ad-156">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-156">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a8ad-157">Пример</span><span class="sxs-lookup"><span data-stu-id="0a8ad-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a8ad-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a8ad-158">Request</span></span>
<span data-ttu-id="0a8ad-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess
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

### <a name="response"></a><span data-ttu-id="0a8ad-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a8ad-160">Response</span></span>
<span data-ttu-id="0a8ad-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a8ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




