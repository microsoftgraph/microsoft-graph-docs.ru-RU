---
title: Создание userExperienceAnalyticsDeviceScores
description: Создание нового объекта userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60b7474deb9a9f845f7d90e419e1c5c813dce483
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869070"
---
# <a name="create-userexperienceanalyticsdevicescores"></a><span data-ttu-id="64f9e-103">Создание userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="64f9e-103">Create userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="64f9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64f9e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f9e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64f9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f9e-107">Создание нового [объекта userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="64f9e-107">Create a new [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64f9e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="64f9e-108">Prerequisites</span></span>
<span data-ttu-id="64f9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f9e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64f9e-111">Permission type</span></span>|<span data-ttu-id="64f9e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64f9e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64f9e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64f9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64f9e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64f9e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="64f9e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64f9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64f9e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f9e-116">Not supported.</span></span>|
|<span data-ttu-id="64f9e-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="64f9e-117">Application</span></span>|<span data-ttu-id="64f9e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64f9e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64f9e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64f9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceScores
```

## <a name="request-headers"></a><span data-ttu-id="64f9e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64f9e-120">Request headers</span></span>
|<span data-ttu-id="64f9e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64f9e-121">Header</span></span>|<span data-ttu-id="64f9e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64f9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64f9e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64f9e-123">Authorization</span></span>|<span data-ttu-id="64f9e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64f9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64f9e-125">Accept</span></span>|<span data-ttu-id="64f9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64f9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f9e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64f9e-127">Request body</span></span>
<span data-ttu-id="64f9e-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsDeviceScores.</span><span class="sxs-lookup"><span data-stu-id="64f9e-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceScores object.</span></span>

<span data-ttu-id="64f9e-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsDeviceScores.</span><span class="sxs-lookup"><span data-stu-id="64f9e-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceScores.</span></span>

|<span data-ttu-id="64f9e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64f9e-130">Property</span></span>|<span data-ttu-id="64f9e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64f9e-131">Type</span></span>|<span data-ttu-id="64f9e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64f9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f9e-133">id</span><span class="sxs-lookup"><span data-stu-id="64f9e-133">id</span></span>|<span data-ttu-id="64f9e-134">String</span><span class="sxs-lookup"><span data-stu-id="64f9e-134">String</span></span>|<span data-ttu-id="64f9e-135">Уникальный идентификатор устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="64f9e-135">The unique identifier of the user experience analytics device scores device.</span></span>|
|<span data-ttu-id="64f9e-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="64f9e-136">deviceName</span></span>|<span data-ttu-id="64f9e-137">String</span><span class="sxs-lookup"><span data-stu-id="64f9e-137">String</span></span>|<span data-ttu-id="64f9e-138">Имя устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="64f9e-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="64f9e-139">model</span><span class="sxs-lookup"><span data-stu-id="64f9e-139">model</span></span>|<span data-ttu-id="64f9e-140">String</span><span class="sxs-lookup"><span data-stu-id="64f9e-140">String</span></span>|<span data-ttu-id="64f9e-141">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="64f9e-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="64f9e-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="64f9e-142">manufacturer</span></span>|<span data-ttu-id="64f9e-143">String</span><span class="sxs-lookup"><span data-stu-id="64f9e-143">String</span></span>|<span data-ttu-id="64f9e-144">Производитель устройств аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="64f9e-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="64f9e-145">endpointAnalyticsScore</span><span class="sxs-lookup"><span data-stu-id="64f9e-145">endpointAnalyticsScore</span></span>|<span data-ttu-id="64f9e-146">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f9e-146">Double</span></span>|<span data-ttu-id="64f9e-147">Оценка устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="64f9e-147">The user experience analytics device score.</span></span> <span data-ttu-id="64f9e-148">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="64f9e-148">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="64f9e-149">startupPerformanceScore</span><span class="sxs-lookup"><span data-stu-id="64f9e-149">startupPerformanceScore</span></span>|<span data-ttu-id="64f9e-150">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f9e-150">Double</span></span>|<span data-ttu-id="64f9e-151">Оценка производительности запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="64f9e-151">The user experience analytics device startup performance score.</span></span> <span data-ttu-id="64f9e-152">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="64f9e-152">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="64f9e-153">appReliabilityScore</span><span class="sxs-lookup"><span data-stu-id="64f9e-153">appReliabilityScore</span></span>|<span data-ttu-id="64f9e-154">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f9e-154">Double</span></span>|<span data-ttu-id="64f9e-155">Оценка надежности приложения приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="64f9e-155">The user experience analytics device app reliability score.</span></span> <span data-ttu-id="64f9e-156">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="64f9e-156">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="64f9e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f9e-157">Response</span></span>
<span data-ttu-id="64f9e-158">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="64f9e-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f9e-159">Пример</span><span class="sxs-lookup"><span data-stu-id="64f9e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="64f9e-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="64f9e-160">Request</span></span>
<span data-ttu-id="64f9e-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64f9e-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333
}
```

### <a name="response"></a><span data-ttu-id="64f9e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f9e-162">Response</span></span>
<span data-ttu-id="64f9e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64f9e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333
}
```




