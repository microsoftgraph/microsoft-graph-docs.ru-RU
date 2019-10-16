---
title: Обновление Усерекспериенцеаналитиксрегрессионсуммари
description: Обновление свойств объекта Усерекспериенцеаналитиксрегрессионсуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcc7aab75801de94b292e5cac7bcb6d206b183a1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529104"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="6f3f4-103">Обновление Усерекспериенцеаналитиксрегрессионсуммари</span><span class="sxs-lookup"><span data-stu-id="6f3f4-103">Update userExperienceAnalyticsRegressionSummary</span></span>

> <span data-ttu-id="6f3f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f3f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f3f4-106">Обновление свойств объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="6f3f4-106">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f3f4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f3f4-107">Prerequisites</span></span>
<span data-ttu-id="6f3f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f3f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f3f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f3f4-110">Permission type</span></span>|<span data-ttu-id="6f3f4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f3f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f3f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f3f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f3f4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f3f4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6f3f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f3f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f3f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-115">Not supported.</span></span>|
|<span data-ttu-id="6f3f4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f3f4-116">Application</span></span>|<span data-ttu-id="6f3f4-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f3f4-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f3f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f3f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="6f3f4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f3f4-119">Request headers</span></span>
|<span data-ttu-id="6f3f4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f3f4-120">Header</span></span>|<span data-ttu-id="6f3f4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6f3f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f3f4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f3f4-122">Authorization</span></span>|<span data-ttu-id="6f3f4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f3f4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6f3f4-124">Accept</span></span>|<span data-ttu-id="6f3f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f3f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f3f4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f3f4-126">Request body</span></span>
<span data-ttu-id="6f3f4-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="6f3f4-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6f3f4-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="6f3f4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f3f4-129">Property</span></span>|<span data-ttu-id="6f3f4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6f3f4-130">Type</span></span>|<span data-ttu-id="6f3f4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6f3f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f3f4-132">id</span><span class="sxs-lookup"><span data-stu-id="6f3f4-132">id</span></span>|<span data-ttu-id="6f3f4-133">String</span><span class="sxs-lookup"><span data-stu-id="6f3f4-133">String</span></span>|<span data-ttu-id="6f3f4-134">Уникальный идентификатор сводки по регрессии аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-134">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="6f3f4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f3f4-135">Response</span></span>
<span data-ttu-id="6f3f4-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксрегрессионсуммари](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-136">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f3f4-137">Пример</span><span class="sxs-lookup"><span data-stu-id="6f3f4-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f3f4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f3f4-138">Request</span></span>
<span data-ttu-id="6f3f4-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="6f3f4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f3f4-140">Response</span></span>
<span data-ttu-id="6f3f4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f3f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```






