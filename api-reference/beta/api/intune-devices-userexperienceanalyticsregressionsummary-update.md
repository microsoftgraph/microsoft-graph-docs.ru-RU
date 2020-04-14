---
title: Обновление Усерекспериенцеаналитиксрегрессионсуммари
description: Обновление свойств объекта Усерекспериенцеаналитиксрегрессионсуммари.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bf55cb371c4bf6b59dfd5b6143eeef8a16abc83
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379039"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="77b61-103">Обновление Усерекспериенцеаналитиксрегрессионсуммари</span><span class="sxs-lookup"><span data-stu-id="77b61-103">Update userExperienceAnalyticsRegressionSummary</span></span>

<span data-ttu-id="77b61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77b61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77b61-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77b61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77b61-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77b61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77b61-107">Обновление свойств объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="77b61-107">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77b61-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77b61-108">Prerequisites</span></span>
<span data-ttu-id="77b61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77b61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77b61-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77b61-111">Permission type</span></span>|<span data-ttu-id="77b61-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77b61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77b61-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77b61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77b61-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77b61-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="77b61-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77b61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77b61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77b61-116">Not supported.</span></span>|
|<span data-ttu-id="77b61-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="77b61-117">Application</span></span>|<span data-ttu-id="77b61-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77b61-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77b61-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77b61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="77b61-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77b61-120">Request headers</span></span>
|<span data-ttu-id="77b61-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77b61-121">Header</span></span>|<span data-ttu-id="77b61-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77b61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77b61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77b61-123">Authorization</span></span>|<span data-ttu-id="77b61-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77b61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77b61-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77b61-125">Accept</span></span>|<span data-ttu-id="77b61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77b61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77b61-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77b61-127">Request body</span></span>
<span data-ttu-id="77b61-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77b61-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="77b61-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span><span class="sxs-lookup"><span data-stu-id="77b61-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="77b61-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77b61-130">Property</span></span>|<span data-ttu-id="77b61-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77b61-131">Type</span></span>|<span data-ttu-id="77b61-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77b61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77b61-133">id</span><span class="sxs-lookup"><span data-stu-id="77b61-133">id</span></span>|<span data-ttu-id="77b61-134">String</span><span class="sxs-lookup"><span data-stu-id="77b61-134">String</span></span>|<span data-ttu-id="77b61-135">Уникальный идентификатор сводки по регрессии аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="77b61-135">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="77b61-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="77b61-136">Response</span></span>
<span data-ttu-id="77b61-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77b61-137">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77b61-138">Пример</span><span class="sxs-lookup"><span data-stu-id="77b61-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="77b61-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="77b61-139">Request</span></span>
<span data-ttu-id="77b61-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77b61-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="77b61-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="77b61-141">Response</span></span>
<span data-ttu-id="77b61-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77b61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```



