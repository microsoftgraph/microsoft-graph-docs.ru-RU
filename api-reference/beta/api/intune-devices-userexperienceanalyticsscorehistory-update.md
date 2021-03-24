---
title: Обновление userExperienceAnalyticsScoreHistory
description: Обновление свойств объекта userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 932e990ca028cee40220fb5e49b0d9353a1c577a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146134"
---
# <a name="update-userexperienceanalyticsscorehistory"></a><span data-ttu-id="c2c6f-103">Обновление userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="c2c6f-103">Update userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="c2c6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2c6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2c6f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2c6f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2c6f-107">Обновление свойств объекта [userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="c2c6f-107">Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2c6f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2c6f-108">Prerequisites</span></span>
<span data-ttu-id="c2c6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2c6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2c6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2c6f-111">Permission type</span></span>|<span data-ttu-id="c2c6f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2c6f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2c6f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2c6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2c6f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2c6f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c2c6f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2c6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2c6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-116">Not supported.</span></span>|
|<span data-ttu-id="c2c6f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2c6f-117">Application</span></span>|<span data-ttu-id="c2c6f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2c6f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2c6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2c6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="c2c6f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2c6f-120">Request headers</span></span>
|<span data-ttu-id="c2c6f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2c6f-121">Header</span></span>|<span data-ttu-id="c2c6f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2c6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2c6f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2c6f-123">Authorization</span></span>|<span data-ttu-id="c2c6f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2c6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2c6f-125">Accept</span></span>|<span data-ttu-id="c2c6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2c6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2c6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2c6f-127">Request body</span></span>
<span data-ttu-id="c2c6f-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="c2c6f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

<span data-ttu-id="c2c6f-129">В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="c2c6f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span></span>

|<span data-ttu-id="c2c6f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2c6f-130">Property</span></span>|<span data-ttu-id="c2c6f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2c6f-131">Type</span></span>|<span data-ttu-id="c2c6f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2c6f-133">id</span><span class="sxs-lookup"><span data-stu-id="c2c6f-133">id</span></span>|<span data-ttu-id="c2c6f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c2c6f-134">String</span></span>|<span data-ttu-id="c2c6f-135">Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="c2c6f-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="c2c6f-136">startupDateTime</span></span>|<span data-ttu-id="c2c6f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2c6f-137">DateTimeOffset</span></span>|<span data-ttu-id="c2c6f-138">Время запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="c2c6f-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="c2c6f-139">startupScore</span></span>|<span data-ttu-id="c2c6f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c2c6f-140">Int32</span></span>|<span data-ttu-id="c2c6f-141">Оценка запуска устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-141">User experience analytics device startup score.</span></span> <span data-ttu-id="c2c6f-142">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-142">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="c2c6f-143">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="c2c6f-143">coreBootScore</span></span>|<span data-ttu-id="c2c6f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c2c6f-144">Int32</span></span>|<span data-ttu-id="c2c6f-145">Оценка загрузки основного загрузочного устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-145">The user experience analytics device core boot score.</span></span> <span data-ttu-id="c2c6f-146">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-146">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="c2c6f-147">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="c2c6f-147">coreSigninScore</span></span>|<span data-ttu-id="c2c6f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c2c6f-148">Int32</span></span>|<span data-ttu-id="c2c6f-149">Оценка основного входного знака устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-149">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="c2c6f-150">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-150">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="c2c6f-151">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="c2c6f-151">recommendedSoftwareScore</span></span>|<span data-ttu-id="c2c6f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c2c6f-152">Int32</span></span>|<span data-ttu-id="c2c6f-153">Оценка основного входного знака устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-153">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="c2c6f-154">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-154">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="c2c6f-155">restartScore</span><span class="sxs-lookup"><span data-stu-id="c2c6f-155">restartScore</span></span>|<span data-ttu-id="c2c6f-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c2c6f-156">Int32</span></span>|<span data-ttu-id="c2c6f-157">Оценка перезапуска.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-157">Restart score.</span></span> <span data-ttu-id="c2c6f-158">Оценка будет в диапазоне 0-100, 100 является идеальным показателем, 0 указывает на чрезмерные перезапуски.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-158">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="c2c6f-159">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="c2c6f-159">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="c2c6f-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2c6f-160">Response</span></span>
<span data-ttu-id="c2c6f-161">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2c6f-162">Пример</span><span class="sxs-lookup"><span data-stu-id="c2c6f-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2c6f-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2c6f-163">Request</span></span>
<span data-ttu-id="c2c6f-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```

### <a name="response"></a><span data-ttu-id="c2c6f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2c6f-165">Response</span></span>
<span data-ttu-id="c2c6f-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2c6f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "restartScore": 12
}
```




