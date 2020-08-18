---
title: Обновление Усерекспериенцеаналитиксметричистори
description: Обновление свойств объекта Усерекспериенцеаналитиксметричистори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a7d0689c1ecd3ff72f1b7d3d1f33366bfbed8f4
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793532"
---
# <a name="update-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="3b44e-103">Обновление Усерекспериенцеаналитиксметричистори</span><span class="sxs-lookup"><span data-stu-id="3b44e-103">Update userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="3b44e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b44e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b44e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b44e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b44e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b44e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b44e-107">Обновление свойств объекта [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) .</span><span class="sxs-lookup"><span data-stu-id="3b44e-107">Update the properties of a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b44e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b44e-108">Prerequisites</span></span>
<span data-ttu-id="3b44e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b44e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b44e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b44e-111">Permission type</span></span>|<span data-ttu-id="3b44e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b44e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b44e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b44e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b44e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b44e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b44e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b44e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b44e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b44e-116">Not supported.</span></span>|
|<span data-ttu-id="3b44e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3b44e-117">Application</span></span>|<span data-ttu-id="3b44e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b44e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b44e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b44e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="3b44e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b44e-120">Request headers</span></span>
|<span data-ttu-id="3b44e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b44e-121">Header</span></span>|<span data-ttu-id="3b44e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b44e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b44e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b44e-123">Authorization</span></span>|<span data-ttu-id="3b44e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b44e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b44e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b44e-125">Accept</span></span>|<span data-ttu-id="3b44e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b44e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b44e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b44e-127">Request body</span></span>
<span data-ttu-id="3b44e-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b44e-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

<span data-ttu-id="3b44e-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span><span class="sxs-lookup"><span data-stu-id="3b44e-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span></span>

|<span data-ttu-id="3b44e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b44e-130">Property</span></span>|<span data-ttu-id="3b44e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b44e-131">Type</span></span>|<span data-ttu-id="3b44e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b44e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b44e-133">id</span><span class="sxs-lookup"><span data-stu-id="3b44e-133">id</span></span>|<span data-ttu-id="3b44e-134">String</span><span class="sxs-lookup"><span data-stu-id="3b44e-134">String</span></span>|<span data-ttu-id="3b44e-135">Уникальный идентификатор истории метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="3b44e-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="3b44e-136">метрикдатетиме</span><span class="sxs-lookup"><span data-stu-id="3b44e-136">metricDateTime</span></span>|<span data-ttu-id="3b44e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b44e-137">DateTimeOffset</span></span>|<span data-ttu-id="3b44e-138">Дата и время метрики аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="3b44e-138">The user experience analytics metric date time.</span></span>|



## <a name="response"></a><span data-ttu-id="3b44e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b44e-139">Response</span></span>
<span data-ttu-id="3b44e-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксметричистори](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b44e-140">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b44e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="3b44e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b44e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b44e-142">Request</span></span>
<span data-ttu-id="3b44e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b44e-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
Content-type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3b44e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b44e-144">Response</span></span>
<span data-ttu-id="3b44e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b44e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 185

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00"
}
```



