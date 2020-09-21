---
title: Создание Усерекспериенцеаналитиксметричистори
description: Создание нового объекта Усерекспериенцеаналитиксметричистори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b5f02c4cb7558c3c3e18661e3978a16227d23b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970112"
---
# <a name="create-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="8ee87-103">Создание Усерекспериенцеаналитиксметричистори</span><span class="sxs-lookup"><span data-stu-id="8ee87-103">Create userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="8ee87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ee87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ee87-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ee87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ee87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ee87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ee87-107">Создание нового объекта [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .</span><span class="sxs-lookup"><span data-stu-id="8ee87-107">Create a new [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ee87-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ee87-108">Prerequisites</span></span>
<span data-ttu-id="8ee87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ee87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ee87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ee87-111">Permission type</span></span>|<span data-ttu-id="8ee87-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ee87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ee87-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ee87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ee87-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee87-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ee87-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ee87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ee87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ee87-116">Not supported.</span></span>|
|<span data-ttu-id="8ee87-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ee87-117">Application</span></span>|<span data-ttu-id="8ee87-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee87-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ee87-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ee87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsMetricHistory
```

## <a name="request-headers"></a><span data-ttu-id="8ee87-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ee87-120">Request headers</span></span>
|<span data-ttu-id="8ee87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ee87-121">Header</span></span>|<span data-ttu-id="8ee87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ee87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ee87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ee87-123">Authorization</span></span>|<span data-ttu-id="8ee87-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ee87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ee87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ee87-125">Accept</span></span>|<span data-ttu-id="8ee87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ee87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ee87-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ee87-127">Request body</span></span>
<span data-ttu-id="8ee87-128">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксметричистори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ee87-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetricHistory object.</span></span>

<span data-ttu-id="8ee87-129">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксметричистори.</span><span class="sxs-lookup"><span data-stu-id="8ee87-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetricHistory.</span></span>

|<span data-ttu-id="8ee87-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ee87-130">Property</span></span>|<span data-ttu-id="8ee87-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ee87-131">Type</span></span>|<span data-ttu-id="8ee87-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ee87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ee87-133">id</span><span class="sxs-lookup"><span data-stu-id="8ee87-133">id</span></span>|<span data-ttu-id="8ee87-134">String</span><span class="sxs-lookup"><span data-stu-id="8ee87-134">String</span></span>|<span data-ttu-id="8ee87-135">Уникальный идентификатор истории метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ee87-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="8ee87-136">метрикдатетиме</span><span class="sxs-lookup"><span data-stu-id="8ee87-136">metricDateTime</span></span>|<span data-ttu-id="8ee87-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ee87-137">DateTimeOffset</span></span>|<span data-ttu-id="8ee87-138">Дата и время метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ee87-138">The user experience analytics metric date time.</span></span>|



## <a name="response"></a><span data-ttu-id="8ee87-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ee87-139">Response</span></span>
<span data-ttu-id="8ee87-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ee87-140">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ee87-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8ee87-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ee87-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ee87-142">Request</span></span>
<span data-ttu-id="8ee87-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ee87-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8ee87-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ee87-144">Response</span></span>
<span data-ttu-id="8ee87-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ee87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 185

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```






