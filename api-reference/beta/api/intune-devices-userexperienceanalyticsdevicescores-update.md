---
title: Обновление userExperienceAnalyticsDeviceScores
description: Обновление свойств объекта userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd1931354ef212fced101d508bbb4c1bf5a5145d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868803"
---
# <a name="update-userexperienceanalyticsdevicescores"></a><span data-ttu-id="9b6f5-103">Обновление userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="9b6f5-103">Update userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="9b6f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b6f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b6f5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b6f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b6f5-107">Обновление свойств объекта [userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="9b6f5-107">Update the properties of a [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b6f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b6f5-108">Prerequisites</span></span>
<span data-ttu-id="9b6f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b6f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b6f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b6f5-111">Permission type</span></span>|<span data-ttu-id="9b6f5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b6f5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b6f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b6f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b6f5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b6f5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9b6f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b6f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b6f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-116">Not supported.</span></span>|
|<span data-ttu-id="9b6f5-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9b6f5-117">Application</span></span>|<span data-ttu-id="9b6f5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b6f5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b6f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b6f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

## <a name="request-headers"></a><span data-ttu-id="9b6f5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9b6f5-120">Request headers</span></span>
|<span data-ttu-id="9b6f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b6f5-121">Header</span></span>|<span data-ttu-id="9b6f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b6f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b6f5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b6f5-123">Authorization</span></span>|<span data-ttu-id="9b6f5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b6f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b6f5-125">Accept</span></span>|<span data-ttu-id="9b6f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b6f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b6f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b6f5-127">Request body</span></span>
<span data-ttu-id="9b6f5-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="9b6f5-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

<span data-ttu-id="9b6f5-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsDeviceScores.](../resources/intune-devices-userexperienceanalyticsdevicescores.md)</span><span class="sxs-lookup"><span data-stu-id="9b6f5-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md).</span></span>

|<span data-ttu-id="9b6f5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b6f5-130">Property</span></span>|<span data-ttu-id="9b6f5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b6f5-131">Type</span></span>|<span data-ttu-id="9b6f5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b6f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b6f5-133">id</span><span class="sxs-lookup"><span data-stu-id="9b6f5-133">id</span></span>|<span data-ttu-id="9b6f5-134">String</span><span class="sxs-lookup"><span data-stu-id="9b6f5-134">String</span></span>|<span data-ttu-id="9b6f5-135">Уникальный идентификатор устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-135">The unique identifier of the user experience analytics device scores device.</span></span>|
|<span data-ttu-id="9b6f5-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="9b6f5-136">deviceName</span></span>|<span data-ttu-id="9b6f5-137">String</span><span class="sxs-lookup"><span data-stu-id="9b6f5-137">String</span></span>|<span data-ttu-id="9b6f5-138">Имя устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="9b6f5-139">model</span><span class="sxs-lookup"><span data-stu-id="9b6f5-139">model</span></span>|<span data-ttu-id="9b6f5-140">String</span><span class="sxs-lookup"><span data-stu-id="9b6f5-140">String</span></span>|<span data-ttu-id="9b6f5-141">Модель устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="9b6f5-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9b6f5-142">manufacturer</span></span>|<span data-ttu-id="9b6f5-143">String</span><span class="sxs-lookup"><span data-stu-id="9b6f5-143">String</span></span>|<span data-ttu-id="9b6f5-144">Производитель устройств аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="9b6f5-145">endpointAnalyticsScore</span><span class="sxs-lookup"><span data-stu-id="9b6f5-145">endpointAnalyticsScore</span></span>|<span data-ttu-id="9b6f5-146">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="9b6f5-146">Double</span></span>|<span data-ttu-id="9b6f5-147">Оценка устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-147">The user experience analytics device score.</span></span> <span data-ttu-id="9b6f5-148">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="9b6f5-148">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="9b6f5-149">startupPerformanceScore</span><span class="sxs-lookup"><span data-stu-id="9b6f5-149">startupPerformanceScore</span></span>|<span data-ttu-id="9b6f5-150">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="9b6f5-150">Double</span></span>|<span data-ttu-id="9b6f5-151">Оценка производительности запуска устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-151">The user experience analytics device startup performance score.</span></span> <span data-ttu-id="9b6f5-152">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="9b6f5-152">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="9b6f5-153">appReliabilityScore</span><span class="sxs-lookup"><span data-stu-id="9b6f5-153">appReliabilityScore</span></span>|<span data-ttu-id="9b6f5-154">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="9b6f5-154">Double</span></span>|<span data-ttu-id="9b6f5-155">Оценка надежности приложения приложения для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-155">The user experience analytics device app reliability score.</span></span> <span data-ttu-id="9b6f5-156">Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308</span><span class="sxs-lookup"><span data-stu-id="9b6f5-156">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="9b6f5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6f5-157">Response</span></span>
<span data-ttu-id="9b6f5-158">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b6f5-159">Пример</span><span class="sxs-lookup"><span data-stu-id="9b6f5-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b6f5-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b6f5-160">Request</span></span>
<span data-ttu-id="9b6f5-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
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

### <a name="response"></a><span data-ttu-id="9b6f5-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b6f5-162">Response</span></span>
<span data-ttu-id="9b6f5-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b6f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




