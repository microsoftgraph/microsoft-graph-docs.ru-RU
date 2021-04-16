---
title: Обновление userExperienceAnalyticsWorkFromAnywhereMetric
description: Обновление свойств объекта userExperienceAnalyticsWorkFromAnywhereMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e38f85106bf472c9eed7b0a6f1dff806fd075b5d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868995"
---
# <a name="update-userexperienceanalyticsworkfromanywheremetric"></a><span data-ttu-id="fa4d5-103">Обновление userExperienceAnalyticsWorkFromAnywhereMetric</span><span class="sxs-lookup"><span data-stu-id="fa4d5-103">Update userExperienceAnalyticsWorkFromAnywhereMetric</span></span>

<span data-ttu-id="fa4d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa4d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa4d5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa4d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa4d5-107">Обновление свойств объекта [userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)</span><span class="sxs-lookup"><span data-stu-id="fa4d5-107">Update the properties of a [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa4d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa4d5-108">Prerequisites</span></span>
<span data-ttu-id="fa4d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa4d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa4d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa4d5-111">Permission type</span></span>|<span data-ttu-id="fa4d5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa4d5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa4d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa4d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa4d5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa4d5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fa4d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa4d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa4d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-116">Not supported.</span></span>|
|<span data-ttu-id="fa4d5-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fa4d5-117">Application</span></span>|<span data-ttu-id="fa4d5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa4d5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa4d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa4d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="fa4d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa4d5-120">Request headers</span></span>
|<span data-ttu-id="fa4d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa4d5-121">Header</span></span>|<span data-ttu-id="fa4d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa4d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa4d5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa4d5-123">Authorization</span></span>|<span data-ttu-id="fa4d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa4d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa4d5-125">Accept</span></span>|<span data-ttu-id="fa4d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa4d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa4d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa4d5-127">Request body</span></span>
<span data-ttu-id="fa4d5-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)</span><span class="sxs-lookup"><span data-stu-id="fa4d5-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object.</span></span>

<span data-ttu-id="fa4d5-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsWorkFromAnywhereMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md)</span><span class="sxs-lookup"><span data-stu-id="fa4d5-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md).</span></span>

|<span data-ttu-id="fa4d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa4d5-130">Property</span></span>|<span data-ttu-id="fa4d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa4d5-131">Type</span></span>|<span data-ttu-id="fa4d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa4d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa4d5-133">id</span><span class="sxs-lookup"><span data-stu-id="fa4d5-133">id</span></span>|<span data-ttu-id="fa4d5-134">String</span><span class="sxs-lookup"><span data-stu-id="fa4d5-134">String</span></span>|<span data-ttu-id="fa4d5-135">Уникальный идентификатор аналитики пользовательских интерфейсов работает из любой метрики.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-135">The unique identifier of the user experience analytics work from anywhere metric.</span></span>|



## <a name="response"></a><span data-ttu-id="fa4d5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa4d5-136">Response</span></span>
<span data-ttu-id="fa4d5-137">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-137">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa4d5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="fa4d5-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa4d5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa4d5-139">Request</span></span>
<span data-ttu-id="fa4d5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}
Content-type: application/json
Content-length: 87

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric"
}
```

### <a name="response"></a><span data-ttu-id="fa4d5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa4d5-141">Response</span></span>
<span data-ttu-id="fa4d5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa4d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric",
  "id": "7e6fda96-da96-7e6f-96da-6f7e96da6f7e"
}
```




