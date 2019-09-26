---
title: Создание Усерекспериенцеаналитиксметрик
description: Создание нового объекта Усерекспериенцеаналитиксметрик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be303d476524af2711937dd73d8f93d244e05d24
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188201"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="07690-103">Создание Усерекспериенцеаналитиксметрик</span><span class="sxs-lookup"><span data-stu-id="07690-103">Create userExperienceAnalyticsMetric</span></span>

> <span data-ttu-id="07690-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07690-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07690-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07690-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07690-106">Создание нового объекта [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) .</span><span class="sxs-lookup"><span data-stu-id="07690-106">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07690-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07690-107">Prerequisites</span></span>
<span data-ttu-id="07690-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07690-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07690-110">Permission type</span></span>|<span data-ttu-id="07690-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07690-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07690-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07690-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07690-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07690-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="07690-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07690-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07690-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07690-115">Not supported.</span></span>|
|<span data-ttu-id="07690-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07690-116">Application</span></span>|<span data-ttu-id="07690-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07690-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07690-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07690-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="07690-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07690-119">Request headers</span></span>
|<span data-ttu-id="07690-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07690-120">Header</span></span>|<span data-ttu-id="07690-121">Значение</span><span class="sxs-lookup"><span data-stu-id="07690-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07690-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07690-122">Authorization</span></span>|<span data-ttu-id="07690-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07690-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07690-124">Accept</span><span class="sxs-lookup"><span data-stu-id="07690-124">Accept</span></span>|<span data-ttu-id="07690-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07690-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07690-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07690-126">Request body</span></span>
<span data-ttu-id="07690-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксметрик в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07690-127">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="07690-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксметрик.</span><span class="sxs-lookup"><span data-stu-id="07690-128">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="07690-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="07690-129">Property</span></span>|<span data-ttu-id="07690-130">Тип</span><span class="sxs-lookup"><span data-stu-id="07690-130">Type</span></span>|<span data-ttu-id="07690-131">Описание</span><span class="sxs-lookup"><span data-stu-id="07690-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07690-132">id</span><span class="sxs-lookup"><span data-stu-id="07690-132">id</span></span>|<span data-ttu-id="07690-133">String</span><span class="sxs-lookup"><span data-stu-id="07690-133">String</span></span>|<span data-ttu-id="07690-134">Уникальный идентификатор метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="07690-134">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="07690-135">значение</span><span class="sxs-lookup"><span data-stu-id="07690-135">value</span></span>|<span data-ttu-id="07690-136">Двойное</span><span class="sxs-lookup"><span data-stu-id="07690-136">Double</span></span>|<span data-ttu-id="07690-137">Значение метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="07690-137">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="07690-138">устройств</span><span class="sxs-lookup"><span data-stu-id="07690-138">unit</span></span>|<span data-ttu-id="07690-139">String.</span><span class="sxs-lookup"><span data-stu-id="07690-139">String</span></span>|<span data-ttu-id="07690-140">Единица измерения показателя взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="07690-140">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="07690-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="07690-141">Response</span></span>
<span data-ttu-id="07690-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07690-142">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07690-143">Пример</span><span class="sxs-lookup"><span data-stu-id="07690-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="07690-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="07690-144">Request</span></span>
<span data-ttu-id="07690-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07690-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="07690-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="07690-146">Response</span></span>
<span data-ttu-id="07690-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07690-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 196

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```




