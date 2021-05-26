---
title: Обновление userExperienceAnalyticsScoreHistory
description: Обновление свойств объекта userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af10809804f933b9a049ae37dad4aecfa2bf0c9e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666235"
---
# <a name="update-userexperienceanalyticsscorehistory"></a><span data-ttu-id="5b35e-103">Обновление userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="5b35e-103">Update userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="5b35e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b35e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b35e-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b35e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b35e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b35e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b35e-107">Обновление свойств объекта [userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="5b35e-107">Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b35e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b35e-108">Prerequisites</span></span>
<span data-ttu-id="5b35e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b35e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b35e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b35e-111">Permission type</span></span>|<span data-ttu-id="5b35e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b35e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b35e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b35e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b35e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b35e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5b35e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b35e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b35e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b35e-116">Not supported.</span></span>|
|<span data-ttu-id="5b35e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b35e-117">Application</span></span>|<span data-ttu-id="5b35e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b35e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b35e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b35e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5b35e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b35e-120">Request headers</span></span>
|<span data-ttu-id="5b35e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b35e-121">Header</span></span>|<span data-ttu-id="5b35e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b35e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b35e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b35e-123">Authorization</span></span>|<span data-ttu-id="5b35e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b35e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b35e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b35e-125">Accept</span></span>|<span data-ttu-id="5b35e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b35e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b35e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b35e-127">Request body</span></span>
<span data-ttu-id="5b35e-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="5b35e-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

<span data-ttu-id="5b35e-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="5b35e-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span></span>

|<span data-ttu-id="5b35e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b35e-130">Property</span></span>|<span data-ttu-id="5b35e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5b35e-131">Type</span></span>|<span data-ttu-id="5b35e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5b35e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b35e-133">id</span><span class="sxs-lookup"><span data-stu-id="5b35e-133">id</span></span>|<span data-ttu-id="5b35e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5b35e-134">String</span></span>|<span data-ttu-id="5b35e-135">Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5b35e-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="5b35e-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="5b35e-136">startupDateTime</span></span>|<span data-ttu-id="5b35e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b35e-137">DateTimeOffset</span></span>|<span data-ttu-id="5b35e-138">Время запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5b35e-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="5b35e-139">overallScore</span><span class="sxs-lookup"><span data-stu-id="5b35e-139">overallScore</span></span>|<span data-ttu-id="5b35e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5b35e-140">Int32</span></span>|<span data-ttu-id="5b35e-141">Общая оценка аналитики пользовательского опыта.</span><span class="sxs-lookup"><span data-stu-id="5b35e-141">User experience analytics overall score.</span></span> <span data-ttu-id="5b35e-142">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="5b35e-142">Score will be in the range 0-100, 100 is the ideal score.</span></span> <span data-ttu-id="5b35e-143">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="5b35e-143">Valid values 0 to 100</span></span>|
|<span data-ttu-id="5b35e-144">startupScore</span><span class="sxs-lookup"><span data-stu-id="5b35e-144">startupScore</span></span>|<span data-ttu-id="5b35e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5b35e-145">Int32</span></span>|<span data-ttu-id="5b35e-146">Оценка запуска устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="5b35e-146">User experience analytics device startup score.</span></span> <span data-ttu-id="5b35e-147">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="5b35e-147">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="5b35e-148">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="5b35e-148">coreBootScore</span></span>|<span data-ttu-id="5b35e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5b35e-149">Int32</span></span>|<span data-ttu-id="5b35e-150">Оценка загрузки основного загрузочного устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5b35e-150">The user experience analytics device core boot score.</span></span> <span data-ttu-id="5b35e-151">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="5b35e-151">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="5b35e-152">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="5b35e-152">coreSigninScore</span></span>|<span data-ttu-id="5b35e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5b35e-153">Int32</span></span>|<span data-ttu-id="5b35e-154">Оценка основного входного знака устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5b35e-154">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="5b35e-155">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="5b35e-155">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="5b35e-156">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="5b35e-156">recommendedSoftwareScore</span></span>|<span data-ttu-id="5b35e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5b35e-157">Int32</span></span>|<span data-ttu-id="5b35e-158">Оценка основного входного знака устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5b35e-158">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="5b35e-159">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="5b35e-159">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="5b35e-160">restartScore</span><span class="sxs-lookup"><span data-stu-id="5b35e-160">restartScore</span></span>|<span data-ttu-id="5b35e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5b35e-161">Int32</span></span>|<span data-ttu-id="5b35e-162">Оценка перезапуска.</span><span class="sxs-lookup"><span data-stu-id="5b35e-162">Restart score.</span></span> <span data-ttu-id="5b35e-163">Оценка будет в диапазоне 0-100, 100 является идеальным показателем, 0 указывает на чрезмерные перезапуски.</span><span class="sxs-lookup"><span data-stu-id="5b35e-163">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="5b35e-164">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="5b35e-164">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="5b35e-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b35e-165">Response</span></span>
<span data-ttu-id="5b35e-166">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5b35e-166">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b35e-167">Пример</span><span class="sxs-lookup"><span data-stu-id="5b35e-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b35e-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b35e-168">Request</span></span>
<span data-ttu-id="5b35e-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b35e-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```

### <a name="response"></a><span data-ttu-id="5b35e-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b35e-170">Response</span></span>
<span data-ttu-id="5b35e-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b35e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```




