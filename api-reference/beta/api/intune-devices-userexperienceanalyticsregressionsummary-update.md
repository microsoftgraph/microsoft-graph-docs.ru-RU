---
title: Обновление userExperienceAnalyticsRegressionSummary
description: Обновление свойств объекта userExperienceAnalyticsRegressionSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2d2676d03751426a6524d28869300a185f7a4f9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146176"
---
# <a name="update-userexperienceanalyticsregressionsummary"></a><span data-ttu-id="c6b53-103">Обновление userExperienceAnalyticsRegressionSummary</span><span class="sxs-lookup"><span data-stu-id="c6b53-103">Update userExperienceAnalyticsRegressionSummary</span></span>

<span data-ttu-id="c6b53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6b53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6b53-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6b53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6b53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6b53-107">Обновление свойств объекта [userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)</span><span class="sxs-lookup"><span data-stu-id="c6b53-107">Update the properties of a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6b53-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c6b53-108">Prerequisites</span></span>
<span data-ttu-id="c6b53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6b53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6b53-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b53-111">Permission type</span></span>|<span data-ttu-id="c6b53-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6b53-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6b53-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6b53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6b53-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b53-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c6b53-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6b53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6b53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b53-116">Not supported.</span></span>|
|<span data-ttu-id="c6b53-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c6b53-117">Application</span></span>|<span data-ttu-id="c6b53-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b53-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6b53-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6b53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary
```

## <a name="request-headers"></a><span data-ttu-id="c6b53-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c6b53-120">Request headers</span></span>
|<span data-ttu-id="c6b53-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6b53-121">Header</span></span>|<span data-ttu-id="c6b53-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c6b53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6b53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6b53-123">Authorization</span></span>|<span data-ttu-id="c6b53-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6b53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6b53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6b53-125">Accept</span></span>|<span data-ttu-id="c6b53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6b53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6b53-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6b53-127">Request body</span></span>
<span data-ttu-id="c6b53-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)</span><span class="sxs-lookup"><span data-stu-id="c6b53-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object.</span></span>

<span data-ttu-id="c6b53-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsRegressionSummary.](../resources/intune-devices-userexperienceanalyticsregressionsummary.md)</span><span class="sxs-lookup"><span data-stu-id="c6b53-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md).</span></span>

|<span data-ttu-id="c6b53-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6b53-130">Property</span></span>|<span data-ttu-id="c6b53-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c6b53-131">Type</span></span>|<span data-ttu-id="c6b53-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c6b53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6b53-133">id</span><span class="sxs-lookup"><span data-stu-id="c6b53-133">id</span></span>|<span data-ttu-id="c6b53-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c6b53-134">String</span></span>|<span data-ttu-id="c6b53-135">Уникальный идентификатор сводки регрессии аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c6b53-135">The unique identifier of the user experience analytics regression summary.</span></span>|



## <a name="response"></a><span data-ttu-id="c6b53-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6b53-136">Response</span></span>
<span data-ttu-id="c6b53-137">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c6b53-137">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6b53-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c6b53-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6b53-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6b53-139">Request</span></span>
<span data-ttu-id="c6b53-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6b53-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary
Content-type: application/json
Content-length: 82

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary"
}
```

### <a name="response"></a><span data-ttu-id="c6b53-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6b53-141">Response</span></span>
<span data-ttu-id="c6b53-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6b53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 131

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
  "id": "41683327-3327-4168-2733-684127336841"
}
```




