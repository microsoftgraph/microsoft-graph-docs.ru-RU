---
title: Создание Усерекспериенцеаналитиксдевицестартуфистори
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуфистори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d36442808380f408998b8dedaf5d89d45acb0982
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529202"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="88ea8-103">Создание Усерекспериенцеаналитиксдевицестартуфистори</span><span class="sxs-lookup"><span data-stu-id="88ea8-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

> <span data-ttu-id="88ea8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88ea8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88ea8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88ea8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88ea8-106">Создание нового объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .</span><span class="sxs-lookup"><span data-stu-id="88ea8-106">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88ea8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88ea8-107">Prerequisites</span></span>
<span data-ttu-id="88ea8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88ea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88ea8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88ea8-110">Permission type</span></span>|<span data-ttu-id="88ea8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88ea8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88ea8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88ea8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88ea8-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ea8-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88ea8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88ea8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88ea8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88ea8-115">Not supported.</span></span>|
|<span data-ttu-id="88ea8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="88ea8-116">Application</span></span>|<span data-ttu-id="88ea8-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88ea8-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88ea8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88ea8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="88ea8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88ea8-119">Request headers</span></span>
|<span data-ttu-id="88ea8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88ea8-120">Header</span></span>|<span data-ttu-id="88ea8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="88ea8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88ea8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88ea8-122">Authorization</span></span>|<span data-ttu-id="88ea8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88ea8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88ea8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="88ea8-124">Accept</span></span>|<span data-ttu-id="88ea8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88ea8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88ea8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88ea8-126">Request body</span></span>
<span data-ttu-id="88ea8-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуфистори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88ea8-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="88ea8-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуфистори.</span><span class="sxs-lookup"><span data-stu-id="88ea8-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="88ea8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="88ea8-129">Property</span></span>|<span data-ttu-id="88ea8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="88ea8-130">Type</span></span>|<span data-ttu-id="88ea8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="88ea8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ea8-132">id</span><span class="sxs-lookup"><span data-stu-id="88ea8-132">id</span></span>|<span data-ttu-id="88ea8-133">String</span><span class="sxs-lookup"><span data-stu-id="88ea8-133">String</span></span>|<span data-ttu-id="88ea8-134">Уникальный идентификатор журнала запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="88ea8-134">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="88ea8-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="88ea8-135">deviceId</span></span>|<span data-ttu-id="88ea8-136">String</span><span class="sxs-lookup"><span data-stu-id="88ea8-136">String</span></span>|<span data-ttu-id="88ea8-137">Идентификатор устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="88ea8-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="88ea8-138">startTime</span><span class="sxs-lookup"><span data-stu-id="88ea8-138">startTime</span></span>|<span data-ttu-id="88ea8-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ea8-139">DateTimeOffset</span></span>|<span data-ttu-id="88ea8-140">Время начала загрузки устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="88ea8-140">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="88ea8-141">коребуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="88ea8-141">coreBootTimeInMs</span></span>|<span data-ttu-id="88ea8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea8-142">Int32</span></span>|<span data-ttu-id="88ea8-143">Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="88ea8-143">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="88ea8-144">граупполицибуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="88ea8-144">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="88ea8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea8-145">Int32</span></span>|<span data-ttu-id="88ea8-146">Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="88ea8-146">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="88ea8-147">феатуреупдатебуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="88ea8-147">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="88ea8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea8-148">Int32</span></span>|<span data-ttu-id="88ea8-149">Время обновления компонента службы аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="88ea8-149">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="88ea8-150">тоталбуттимеинмс</span><span class="sxs-lookup"><span data-stu-id="88ea8-150">totalBootTimeInMs</span></span>|<span data-ttu-id="88ea8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea8-151">Int32</span></span>|<span data-ttu-id="88ea8-152">Общее время загрузки устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="88ea8-152">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="88ea8-153">граупполицилогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="88ea8-153">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="88ea8-154">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea8-154">Int32</span></span>|<span data-ttu-id="88ea8-155">Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="88ea8-155">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="88ea8-156">корелогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="88ea8-156">coreLoginTimeInMs</span></span>|<span data-ttu-id="88ea8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea8-157">Int32</span></span>|<span data-ttu-id="88ea8-158">Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="88ea8-158">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="88ea8-159">тоталлогинтимеинмс</span><span class="sxs-lookup"><span data-stu-id="88ea8-159">totalLoginTimeInMs</span></span>|<span data-ttu-id="88ea8-160">Int32</span><span class="sxs-lookup"><span data-stu-id="88ea8-160">Int32</span></span>|<span data-ttu-id="88ea8-161">Общее время входа в систему для устройства аналитики взаимодействия с пользователем (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="88ea8-161">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="88ea8-162">исфирстлогин</span><span class="sxs-lookup"><span data-stu-id="88ea8-162">isFirstLogin</span></span>|<span data-ttu-id="88ea8-163">Логический</span><span class="sxs-lookup"><span data-stu-id="88ea8-163">Boolean</span></span>|<span data-ttu-id="88ea8-164">Первое имя входа устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="88ea8-164">The user experience analytics device first login.</span></span>|



## <a name="response"></a><span data-ttu-id="88ea8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="88ea8-165">Response</span></span>
<span data-ttu-id="88ea8-166">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88ea8-166">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88ea8-167">Пример</span><span class="sxs-lookup"><span data-stu-id="88ea8-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="88ea8-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="88ea8-168">Request</span></span>
<span data-ttu-id="88ea8-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88ea8-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 407

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true
}
```

### <a name="response"></a><span data-ttu-id="88ea8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="88ea8-170">Response</span></span>
<span data-ttu-id="88ea8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88ea8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 456

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true
}
```






