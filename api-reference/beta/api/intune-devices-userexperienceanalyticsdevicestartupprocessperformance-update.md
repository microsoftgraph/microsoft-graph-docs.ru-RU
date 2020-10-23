---
title: Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце
description: Обновление свойств объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94c3dc76d1b3dd75ec8b88541f78088a10e35b44
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702063"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="5f930-103">Обновление Усерекспериенцеаналитиксдевицестартуппроцессперформанце</span><span class="sxs-lookup"><span data-stu-id="5f930-103">Update userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="5f930-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f930-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f930-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f930-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f930-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f930-107">Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="5f930-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f930-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f930-108">Prerequisites</span></span>
<span data-ttu-id="5f930-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f930-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f930-111">Permission type</span></span>|<span data-ttu-id="5f930-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f930-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f930-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f930-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f930-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f930-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5f930-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f930-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f930-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f930-116">Not supported.</span></span>|
|<span data-ttu-id="5f930-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f930-117">Application</span></span>|<span data-ttu-id="5f930-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f930-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f930-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f930-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="5f930-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5f930-120">Request headers</span></span>
|<span data-ttu-id="5f930-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f930-121">Header</span></span>|<span data-ttu-id="5f930-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5f930-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f930-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f930-123">Authorization</span></span>|<span data-ttu-id="5f930-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f930-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f930-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f930-125">Accept</span></span>|<span data-ttu-id="5f930-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f930-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f930-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5f930-127">Request body</span></span>
<span data-ttu-id="5f930-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f930-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

<span data-ttu-id="5f930-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span><span class="sxs-lookup"><span data-stu-id="5f930-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span></span>

|<span data-ttu-id="5f930-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f930-130">Property</span></span>|<span data-ttu-id="5f930-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5f930-131">Type</span></span>|<span data-ttu-id="5f930-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5f930-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f930-133">id</span><span class="sxs-lookup"><span data-stu-id="5f930-133">id</span></span>|<span data-ttu-id="5f930-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5f930-134">String</span></span>|<span data-ttu-id="5f930-135">Уникальный идентификатор производительности процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="5f930-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="5f930-136">процесснаме</span><span class="sxs-lookup"><span data-stu-id="5f930-136">processName</span></span>|<span data-ttu-id="5f930-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5f930-137">String</span></span>|<span data-ttu-id="5f930-138">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="5f930-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="5f930-139">productName</span><span class="sxs-lookup"><span data-stu-id="5f930-139">productName</span></span>|<span data-ttu-id="5f930-140">String</span><span class="sxs-lookup"><span data-stu-id="5f930-140">String</span></span>|<span data-ttu-id="5f930-141">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="5f930-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="5f930-142">publisher</span><span class="sxs-lookup"><span data-stu-id="5f930-142">publisher</span></span>|<span data-ttu-id="5f930-143">String</span><span class="sxs-lookup"><span data-stu-id="5f930-143">String</span></span>|<span data-ttu-id="5f930-144">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="5f930-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="5f930-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5f930-145">deviceCount</span></span>|<span data-ttu-id="5f930-146">Int64</span><span class="sxs-lookup"><span data-stu-id="5f930-146">Int64</span></span>|<span data-ttu-id="5f930-147">Сводка по процессу запуска при запуске устройства с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="5f930-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="5f930-148">медианимпактинмс</span><span class="sxs-lookup"><span data-stu-id="5f930-148">medianImpactInMs</span></span>|<span data-ttu-id="5f930-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5f930-149">Int32</span></span>|<span data-ttu-id="5f930-150">Поведение при запуске устройства Analytics для пользователя в течение среднего влияния в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="5f930-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="5f930-151">тоталимпактинмс</span><span class="sxs-lookup"><span data-stu-id="5f930-151">totalImpactInMs</span></span>|<span data-ttu-id="5f930-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5f930-152">Int32</span></span>|<span data-ttu-id="5f930-153">Общее влияние на процесс запуска пользователя при запуске устройства Analytics (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="5f930-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="5f930-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f930-154">Response</span></span>
<span data-ttu-id="5f930-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f930-155">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f930-156">Пример</span><span class="sxs-lookup"><span data-stu-id="5f930-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f930-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f930-157">Request</span></span>
<span data-ttu-id="5f930-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f930-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5f930-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f930-159">Response</span></span>
<span data-ttu-id="5f930-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f930-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





