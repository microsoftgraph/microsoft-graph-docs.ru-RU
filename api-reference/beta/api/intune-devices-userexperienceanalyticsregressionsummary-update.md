---
title: Обновление Усерекспериенцеаналитиксрегрессионсуммари
description: Обновление свойств объекта Усерекспериенцеаналитиксрегрессионсуммари.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9fa85edbe35ec567557e82330d56cf042d258817
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813784"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="bc33d-103">Обновление Усерекспериенцеаналитиксрегрессионсуммари</span><span class="sxs-lookup"><span data-stu-id="bc33d-103">Update userExperienceAnalyticsRegressionSummary</span></span>

> <span data-ttu-id="bc33d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc33d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc33d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc33d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc33d-106">Обновление свойств объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="bc33d-106">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc33d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bc33d-107">Prerequisites</span></span>
<span data-ttu-id="bc33d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc33d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc33d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc33d-110">Permission type</span></span>|<span data-ttu-id="bc33d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc33d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc33d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc33d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc33d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc33d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bc33d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc33d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc33d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc33d-115">Not supported.</span></span>|
|<span data-ttu-id="bc33d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bc33d-116">Application</span></span>|<span data-ttu-id="bc33d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc33d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc33d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc33d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="bc33d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bc33d-119">Request headers</span></span>
|<span data-ttu-id="bc33d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc33d-120">Header</span></span>|<span data-ttu-id="bc33d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bc33d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc33d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc33d-122">Authorization</span></span>|<span data-ttu-id="bc33d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc33d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc33d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bc33d-124">Accept</span></span>|<span data-ttu-id="bc33d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc33d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc33d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc33d-126">Request body</span></span>
<span data-ttu-id="bc33d-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc33d-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="bc33d-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bc33d-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="bc33d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc33d-129">Property</span></span>|<span data-ttu-id="bc33d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bc33d-130">Type</span></span>|<span data-ttu-id="bc33d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bc33d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc33d-132">id</span><span class="sxs-lookup"><span data-stu-id="bc33d-132">id</span></span>|<span data-ttu-id="bc33d-133">String</span><span class="sxs-lookup"><span data-stu-id="bc33d-133">String</span></span>|<span data-ttu-id="bc33d-134">Уникальный идентификатор сводки по регрессии аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="bc33d-134">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="bc33d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc33d-135">Response</span></span>
<span data-ttu-id="bc33d-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc33d-136">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc33d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="bc33d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc33d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc33d-138">Request</span></span>
<span data-ttu-id="bc33d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc33d-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="bc33d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc33d-140">Response</span></span>
<span data-ttu-id="bc33d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc33d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```




