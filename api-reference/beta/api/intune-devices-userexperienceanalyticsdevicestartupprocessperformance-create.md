---
title: Создание Усерекспериенцеаналитиксдевицестартуппроцессперформанце
description: Создание нового объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1f87169ff1477aae7d64e8fe4fce65df926df8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468252"
---
# <a name="create-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="940df-103">Создание Усерекспериенцеаналитиксдевицестартуппроцессперформанце</span><span class="sxs-lookup"><span data-stu-id="940df-103">Create userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="940df-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="940df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="940df-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="940df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="940df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="940df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="940df-107">Создание нового объекта [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) .</span><span class="sxs-lookup"><span data-stu-id="940df-107">Create a new [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="940df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="940df-108">Prerequisites</span></span>
<span data-ttu-id="940df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="940df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="940df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="940df-111">Permission type</span></span>|<span data-ttu-id="940df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="940df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="940df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="940df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="940df-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940df-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="940df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="940df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="940df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="940df-116">Not supported.</span></span>|
|<span data-ttu-id="940df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="940df-117">Application</span></span>|<span data-ttu-id="940df-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940df-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="940df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="940df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="940df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="940df-120">Request headers</span></span>
|<span data-ttu-id="940df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="940df-121">Header</span></span>|<span data-ttu-id="940df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="940df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="940df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="940df-123">Authorization</span></span>|<span data-ttu-id="940df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="940df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="940df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="940df-125">Accept</span></span>|<span data-ttu-id="940df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="940df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="940df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="940df-127">Request body</span></span>
<span data-ttu-id="940df-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксдевицестартуппроцессперформанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="940df-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcessPerformance object.</span></span>

<span data-ttu-id="940df-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксдевицестартуппроцессперформанце.</span><span class="sxs-lookup"><span data-stu-id="940df-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcessPerformance.</span></span>

|<span data-ttu-id="940df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="940df-130">Property</span></span>|<span data-ttu-id="940df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="940df-131">Type</span></span>|<span data-ttu-id="940df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="940df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="940df-133">id</span><span class="sxs-lookup"><span data-stu-id="940df-133">id</span></span>|<span data-ttu-id="940df-134">String</span><span class="sxs-lookup"><span data-stu-id="940df-134">String</span></span>|<span data-ttu-id="940df-135">Уникальный идентификатор производительности процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="940df-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="940df-136">процесснаме</span><span class="sxs-lookup"><span data-stu-id="940df-136">processName</span></span>|<span data-ttu-id="940df-137">String</span><span class="sxs-lookup"><span data-stu-id="940df-137">String</span></span>|<span data-ttu-id="940df-138">Имя процесса запуска устройства службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="940df-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="940df-139">productName</span><span class="sxs-lookup"><span data-stu-id="940df-139">productName</span></span>|<span data-ttu-id="940df-140">String</span><span class="sxs-lookup"><span data-stu-id="940df-140">String</span></span>|<span data-ttu-id="940df-141">Имя продукта для процесса запуска устройства Analytics Device (взаимодействие с пользователем).</span><span class="sxs-lookup"><span data-stu-id="940df-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="940df-142">publisher</span><span class="sxs-lookup"><span data-stu-id="940df-142">publisher</span></span>|<span data-ttu-id="940df-143">String</span><span class="sxs-lookup"><span data-stu-id="940df-143">String</span></span>|<span data-ttu-id="940df-144">Издатель процесса запуска устройства Analytics User Experience.</span><span class="sxs-lookup"><span data-stu-id="940df-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="940df-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="940df-145">deviceCount</span></span>|<span data-ttu-id="940df-146">Int64</span><span class="sxs-lookup"><span data-stu-id="940df-146">Int64</span></span>|<span data-ttu-id="940df-147">Сводка по процессу запуска при запуске устройства с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="940df-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="940df-148">медианимпактинмс</span><span class="sxs-lookup"><span data-stu-id="940df-148">medianImpactInMs</span></span>|<span data-ttu-id="940df-149">Int32</span><span class="sxs-lookup"><span data-stu-id="940df-149">Int32</span></span>|<span data-ttu-id="940df-150">Поведение при запуске устройства Analytics для пользователя в течение среднего влияния в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="940df-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="940df-151">тоталимпактинмс</span><span class="sxs-lookup"><span data-stu-id="940df-151">totalImpactInMs</span></span>|<span data-ttu-id="940df-152">Int32</span><span class="sxs-lookup"><span data-stu-id="940df-152">Int32</span></span>|<span data-ttu-id="940df-153">Общее влияние на процесс запуска пользователя при запуске устройства Analytics (в миллисекундах).</span><span class="sxs-lookup"><span data-stu-id="940df-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="940df-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="940df-154">Response</span></span>
<span data-ttu-id="940df-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксдевицестартуппроцессперформанце](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="940df-155">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="940df-156">Пример</span><span class="sxs-lookup"><span data-stu-id="940df-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="940df-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="940df-157">Request</span></span>
<span data-ttu-id="940df-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="940df-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="940df-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="940df-159">Response</span></span>
<span data-ttu-id="940df-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="940df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





