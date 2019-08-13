---
title: Обновление Усерекспериенцеаналитиксбаселине
description: Обновление свойств объекта Усерекспериенцеаналитиксбаселине.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: acf31ba513ba45dad93158955a743eafd5848329
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350492"
---
# <a name="update-userexperienceanalyticsbaseline"></a><span data-ttu-id="13c73-103">Обновление Усерекспериенцеаналитиксбаселине</span><span class="sxs-lookup"><span data-stu-id="13c73-103">Update userExperienceAnalyticsBaseline</span></span>

> <span data-ttu-id="13c73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13c73-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13c73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c73-106">Обновление свойств объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) .</span><span class="sxs-lookup"><span data-stu-id="13c73-106">Update the properties of a [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13c73-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13c73-107">Prerequisites</span></span>
<span data-ttu-id="13c73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13c73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13c73-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13c73-110">Permission type</span></span>|<span data-ttu-id="13c73-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13c73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13c73-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13c73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13c73-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c73-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13c73-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13c73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13c73-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c73-115">Not supported.</span></span>|
|<span data-ttu-id="13c73-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13c73-116">Application</span></span>|<span data-ttu-id="13c73-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13c73-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13c73-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13c73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
```

## <a name="request-headers"></a><span data-ttu-id="13c73-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13c73-119">Request headers</span></span>
|<span data-ttu-id="13c73-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13c73-120">Header</span></span>|<span data-ttu-id="13c73-121">Значение</span><span class="sxs-lookup"><span data-stu-id="13c73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13c73-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13c73-122">Authorization</span></span>|<span data-ttu-id="13c73-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13c73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13c73-124">Accept</span><span class="sxs-lookup"><span data-stu-id="13c73-124">Accept</span></span>|<span data-ttu-id="13c73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13c73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c73-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13c73-126">Request body</span></span>
<span data-ttu-id="13c73-127">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13c73-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object.</span></span>

<span data-ttu-id="13c73-128">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span><span class="sxs-lookup"><span data-stu-id="13c73-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md).</span></span>

|<span data-ttu-id="13c73-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="13c73-129">Property</span></span>|<span data-ttu-id="13c73-130">Тип</span><span class="sxs-lookup"><span data-stu-id="13c73-130">Type</span></span>|<span data-ttu-id="13c73-131">Описание</span><span class="sxs-lookup"><span data-stu-id="13c73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13c73-132">id</span><span class="sxs-lookup"><span data-stu-id="13c73-132">id</span></span>|<span data-ttu-id="13c73-133">String</span><span class="sxs-lookup"><span data-stu-id="13c73-133">String</span></span>|<span data-ttu-id="13c73-134">Уникальный идентификатор базового идентификатора аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="13c73-134">The unique identifier of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="13c73-135">displayName</span><span class="sxs-lookup"><span data-stu-id="13c73-135">displayName</span></span>|<span data-ttu-id="13c73-136">Строка</span><span class="sxs-lookup"><span data-stu-id="13c73-136">String</span></span>|<span data-ttu-id="13c73-137">Имя базового объекта аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="13c73-137">The name of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="13c73-138">овераллскоре</span><span class="sxs-lookup"><span data-stu-id="13c73-138">overallScore</span></span>|<span data-ttu-id="13c73-139">Int32</span><span class="sxs-lookup"><span data-stu-id="13c73-139">Int32</span></span>|<span data-ttu-id="13c73-140">Общий показатель базового уровня для аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="13c73-140">The overall score of the user experience analytics baseline.</span></span>|
|<span data-ttu-id="13c73-141">овераллрегрессионсрешолд</span><span class="sxs-lookup"><span data-stu-id="13c73-141">overallRegressionThreshold</span></span>|<span data-ttu-id="13c73-142">Int32</span><span class="sxs-lookup"><span data-stu-id="13c73-142">Int32</span></span>|<span data-ttu-id="13c73-143">Общее пороговое значение базовой регрессии базового интерфейса аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="13c73-143">The overall regression threshold of the user experience analytics baseline.</span></span>|



## <a name="response"></a><span data-ttu-id="13c73-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c73-144">Response</span></span>
<span data-ttu-id="13c73-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксбаселине](../resources/intune-devices-userexperienceanalyticsbaseline.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13c73-145">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13c73-146">Пример</span><span class="sxs-lookup"><span data-stu-id="13c73-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="13c73-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="13c73-147">Request</span></span>
<span data-ttu-id="13c73-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13c73-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "displayName": "Display Name value",
  "overallScore": 12,
  "overallRegressionThreshold": 10
}
```

### <a name="response"></a><span data-ttu-id="13c73-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c73-149">Response</span></span>
<span data-ttu-id="13c73-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13c73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "1cce2cab-2cab-1cce-ab2c-ce1cab2cce1c",
  "displayName": "Display Name value",
  "overallScore": 12,
  "overallRegressionThreshold": 10
}
```






