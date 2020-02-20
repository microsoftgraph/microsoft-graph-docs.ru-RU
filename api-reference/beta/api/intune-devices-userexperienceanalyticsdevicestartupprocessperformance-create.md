---
title: Создание Усерекспериенцеаналитиксдевицестартуппроцессперформанце
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d21d0e2a2289178bf85ee9fddcabc2c7699859ef
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161975"
---
# <a name="create-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="f9ac5-103">Создание Усерекспериенцеаналитиксдевицестартуппроцессперформанце</span><span class="sxs-lookup"><span data-stu-id="f9ac5-103">Create userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

> <span data-ttu-id="f9ac5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9ac5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ac5-106">Создание нового объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="f9ac5-106">Create a new [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9ac5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9ac5-107">Prerequisites</span></span>
<span data-ttu-id="f9ac5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ac5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ac5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9ac5-110">Permission type</span></span>|<span data-ttu-id="f9ac5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9ac5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9ac5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9ac5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9ac5-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ac5-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9ac5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9ac5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9ac5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-115">Not supported.</span></span>|
|<span data-ttu-id="f9ac5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9ac5-116">Application</span></span>|<span data-ttu-id="f9ac5-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9ac5-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9ac5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9ac5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="f9ac5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f9ac5-119">Request headers</span></span>
|<span data-ttu-id="f9ac5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9ac5-120">Header</span></span>|<span data-ttu-id="f9ac5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9ac5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9ac5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9ac5-122">Authorization</span></span>|<span data-ttu-id="f9ac5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9ac5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f9ac5-124">Accept</span></span>|<span data-ttu-id="f9ac5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9ac5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9ac5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9ac5-126">Request body</span></span>
<span data-ttu-id="f9ac5-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcessPerformance object.</span></span>

<span data-ttu-id="f9ac5-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуппроцессперформанце.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcessPerformance.</span></span>

|<span data-ttu-id="f9ac5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9ac5-129">Property</span></span>|<span data-ttu-id="f9ac5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f9ac5-130">Type</span></span>|<span data-ttu-id="f9ac5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f9ac5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ac5-132">id</span><span class="sxs-lookup"><span data-stu-id="f9ac5-132">id</span></span>|<span data-ttu-id="f9ac5-133">String</span><span class="sxs-lookup"><span data-stu-id="f9ac5-133">String</span></span>|<span data-ttu-id="f9ac5-134">Уникальный идентификатор производительности процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-134">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="f9ac5-135">процесснаме</span><span class="sxs-lookup"><span data-stu-id="f9ac5-135">processName</span></span>|<span data-ttu-id="f9ac5-136">String</span><span class="sxs-lookup"><span data-stu-id="f9ac5-136">String</span></span>|<span data-ttu-id="f9ac5-137">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-137">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="f9ac5-138">productName</span><span class="sxs-lookup"><span data-stu-id="f9ac5-138">productName</span></span>|<span data-ttu-id="f9ac5-139">String</span><span class="sxs-lookup"><span data-stu-id="f9ac5-139">String</span></span>|<span data-ttu-id="f9ac5-140">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="f9ac5-140">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="f9ac5-141">publisher</span><span class="sxs-lookup"><span data-stu-id="f9ac5-141">publisher</span></span>|<span data-ttu-id="f9ac5-142">String</span><span class="sxs-lookup"><span data-stu-id="f9ac5-142">String</span></span>|<span data-ttu-id="f9ac5-143">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-143">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="f9ac5-144">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f9ac5-144">deviceCount</span></span>|<span data-ttu-id="f9ac5-145">Int64</span><span class="sxs-lookup"><span data-stu-id="f9ac5-145">Int64</span></span>|<span data-ttu-id="f9ac5-146">Сводка по процессу запуска при запуске устройства с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-146">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="f9ac5-147">медианимпактинмс</span><span class="sxs-lookup"><span data-stu-id="f9ac5-147">medianImpactInMs</span></span>|<span data-ttu-id="f9ac5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f9ac5-148">Int32</span></span>|<span data-ttu-id="f9ac5-149">Поведение при запуске устройства Analytics для пользователя в течение среднего влияния в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-149">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="f9ac5-150">тоталимпактинмс</span><span class="sxs-lookup"><span data-stu-id="f9ac5-150">totalImpactInMs</span></span>|<span data-ttu-id="f9ac5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f9ac5-151">Int32</span></span>|<span data-ttu-id="f9ac5-152">Общее влияние на процесс запуска пользователя при запуске устройства Analytics (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="f9ac5-152">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="f9ac5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ac5-153">Response</span></span>
<span data-ttu-id="f9ac5-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-154">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9ac5-155">Пример</span><span class="sxs-lookup"><span data-stu-id="f9ac5-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9ac5-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9ac5-156">Request</span></span>
<span data-ttu-id="f9ac5-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9ac5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9ac5-158">Response</span></span>
<span data-ttu-id="f9ac5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9ac5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





