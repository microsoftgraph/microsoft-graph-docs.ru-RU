---
title: Создание userExperienceAnalyticsMetricHistory
description: Создание объекта userExperienceAnalyticsMetricHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 070c34b225ab49eb7625c313544a785d7cc3e518
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155057"
---
# <a name="create-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="15298-103">Создание userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="15298-103">Create userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="15298-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15298-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15298-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15298-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15298-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15298-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15298-107">Создание объекта [userExperienceAnalyticsMetricHistory.](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)</span><span class="sxs-lookup"><span data-stu-id="15298-107">Create a new [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15298-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15298-108">Prerequisites</span></span>
<span data-ttu-id="15298-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15298-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15298-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15298-111">Permission type</span></span>|<span data-ttu-id="15298-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15298-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15298-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15298-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15298-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15298-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="15298-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15298-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15298-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15298-116">Not supported.</span></span>|
|<span data-ttu-id="15298-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15298-117">Application</span></span>|<span data-ttu-id="15298-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15298-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15298-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15298-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="15298-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15298-120">Request headers</span></span>
|<span data-ttu-id="15298-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15298-121">Header</span></span>|<span data-ttu-id="15298-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15298-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15298-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15298-123">Authorization</span></span>|<span data-ttu-id="15298-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15298-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15298-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15298-125">Accept</span></span>|<span data-ttu-id="15298-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15298-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15298-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15298-127">Request body</span></span>
<span data-ttu-id="15298-128">В теле запроса укажу представление объекта userExperienceAnalyticsMetricHistory в JSON.</span><span class="sxs-lookup"><span data-stu-id="15298-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetricHistory object.</span></span>

<span data-ttu-id="15298-129">В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsMetricHistory.</span><span class="sxs-lookup"><span data-stu-id="15298-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetricHistory.</span></span>

|<span data-ttu-id="15298-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15298-130">Property</span></span>|<span data-ttu-id="15298-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15298-131">Type</span></span>|<span data-ttu-id="15298-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15298-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15298-133">id</span><span class="sxs-lookup"><span data-stu-id="15298-133">id</span></span>|<span data-ttu-id="15298-134">String</span><span class="sxs-lookup"><span data-stu-id="15298-134">String</span></span>|<span data-ttu-id="15298-135">Уникальный идентификатор истории показателей аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="15298-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="15298-136">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="15298-136">metricDateTime</span></span>|<span data-ttu-id="15298-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15298-137">DateTimeOffset</span></span>|<span data-ttu-id="15298-138">Дата даты анализа пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="15298-138">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="15298-139">metricType</span><span class="sxs-lookup"><span data-stu-id="15298-139">metricType</span></span>|<span data-ttu-id="15298-140">String</span><span class="sxs-lookup"><span data-stu-id="15298-140">String</span></span>|<span data-ttu-id="15298-141">Тип метрики аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="15298-141">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="15298-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="15298-142">Response</span></span>
<span data-ttu-id="15298-143">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15298-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15298-144">Пример</span><span class="sxs-lookup"><span data-stu-id="15298-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="15298-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="15298-145">Request</span></span>
<span data-ttu-id="15298-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15298-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="15298-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="15298-147">Response</span></span>
<span data-ttu-id="15298-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15298-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```




