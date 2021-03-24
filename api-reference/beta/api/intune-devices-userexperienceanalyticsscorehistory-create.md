---
title: Создание userExperienceAnalyticsScoreHistory
description: Создание нового объекта userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f161e58e8ce571d0c4f83e6dcf7b77683e94d70d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146162"
---
# <a name="create-userexperienceanalyticsscorehistory"></a><span data-ttu-id="8fa2a-103">Создание userExperienceAnalyticsScoreHistory</span><span class="sxs-lookup"><span data-stu-id="8fa2a-103">Create userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="8fa2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fa2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fa2a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fa2a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fa2a-107">Создание нового [объекта userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)</span><span class="sxs-lookup"><span data-stu-id="8fa2a-107">Create a new [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fa2a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8fa2a-108">Prerequisites</span></span>
<span data-ttu-id="8fa2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fa2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fa2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fa2a-111">Permission type</span></span>|<span data-ttu-id="8fa2a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fa2a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fa2a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fa2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fa2a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fa2a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8fa2a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fa2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fa2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-116">Not supported.</span></span>|
|<span data-ttu-id="8fa2a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8fa2a-117">Application</span></span>|<span data-ttu-id="8fa2a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fa2a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fa2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fa2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="8fa2a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8fa2a-120">Request headers</span></span>
|<span data-ttu-id="8fa2a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fa2a-121">Header</span></span>|<span data-ttu-id="8fa2a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8fa2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fa2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fa2a-123">Authorization</span></span>|<span data-ttu-id="8fa2a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fa2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8fa2a-125">Accept</span></span>|<span data-ttu-id="8fa2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fa2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fa2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fa2a-127">Request body</span></span>
<span data-ttu-id="8fa2a-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-128">In the request body, supply a JSON representation for the userExperienceAnalyticsScoreHistory object.</span></span>

<span data-ttu-id="8fa2a-129">В следующей таблице показаны свойства, необходимые при создании пользовательского интерфейсаExperienceAnalyticsScoreHistory.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-129">The following table shows the properties that are required when you create the userExperienceAnalyticsScoreHistory.</span></span>

|<span data-ttu-id="8fa2a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fa2a-130">Property</span></span>|<span data-ttu-id="8fa2a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8fa2a-131">Type</span></span>|<span data-ttu-id="8fa2a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8fa2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fa2a-133">id</span><span class="sxs-lookup"><span data-stu-id="8fa2a-133">id</span></span>|<span data-ttu-id="8fa2a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8fa2a-134">String</span></span>|<span data-ttu-id="8fa2a-135">Уникальный идентификатор процесса запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="8fa2a-136">startupDateTime</span><span class="sxs-lookup"><span data-stu-id="8fa2a-136">startupDateTime</span></span>|<span data-ttu-id="8fa2a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fa2a-137">DateTimeOffset</span></span>|<span data-ttu-id="8fa2a-138">Время запуска устройства аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="8fa2a-139">startupScore</span><span class="sxs-lookup"><span data-stu-id="8fa2a-139">startupScore</span></span>|<span data-ttu-id="8fa2a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8fa2a-140">Int32</span></span>|<span data-ttu-id="8fa2a-141">Оценка запуска устройства аналитики пользовательских интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-141">User experience analytics device startup score.</span></span> <span data-ttu-id="8fa2a-142">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-142">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8fa2a-143">coreBootScore</span><span class="sxs-lookup"><span data-stu-id="8fa2a-143">coreBootScore</span></span>|<span data-ttu-id="8fa2a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8fa2a-144">Int32</span></span>|<span data-ttu-id="8fa2a-145">Оценка загрузки основного загрузочного устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-145">The user experience analytics device core boot score.</span></span> <span data-ttu-id="8fa2a-146">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-146">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8fa2a-147">coreSigninScore</span><span class="sxs-lookup"><span data-stu-id="8fa2a-147">coreSigninScore</span></span>|<span data-ttu-id="8fa2a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8fa2a-148">Int32</span></span>|<span data-ttu-id="8fa2a-149">Оценка основного входного знака устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-149">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="8fa2a-150">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-150">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8fa2a-151">recommendedSoftwareScore</span><span class="sxs-lookup"><span data-stu-id="8fa2a-151">recommendedSoftwareScore</span></span>|<span data-ttu-id="8fa2a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8fa2a-152">Int32</span></span>|<span data-ttu-id="8fa2a-153">Оценка основного входного знака устройства для аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-153">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="8fa2a-154">Оценка будет в диапазоне 0-100, 100 является идеальным показателем.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-154">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="8fa2a-155">restartScore</span><span class="sxs-lookup"><span data-stu-id="8fa2a-155">restartScore</span></span>|<span data-ttu-id="8fa2a-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8fa2a-156">Int32</span></span>|<span data-ttu-id="8fa2a-157">Оценка перезапуска.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-157">Restart score.</span></span> <span data-ttu-id="8fa2a-158">Оценка будет в диапазоне 0-100, 100 является идеальным показателем, 0 указывает на чрезмерные перезапуски.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-158">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="8fa2a-159">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="8fa2a-159">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="8fa2a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fa2a-160">Response</span></span>
<span data-ttu-id="8fa2a-161">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fa2a-162">Пример</span><span class="sxs-lookup"><span data-stu-id="8fa2a-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fa2a-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fa2a-163">Request</span></span>
<span data-ttu-id="8fa2a-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory
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

### <a name="response"></a><span data-ttu-id="8fa2a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fa2a-165">Response</span></span>
<span data-ttu-id="8fa2a-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fa2a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




