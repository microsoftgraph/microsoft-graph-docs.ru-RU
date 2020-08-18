---
title: Обновление Усерекспериенцеаналитиксскорехистори
description: Обновление свойств объекта Усерекспериенцеаналитиксскорехистори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e7179fb0dae2c62b2a416722eaa8d8d27ee321a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46789883"
---
# <a name="update-userexperienceanalyticsscorehistory"></a><span data-ttu-id="f1912-103">Обновление Усерекспериенцеаналитиксскорехистори</span><span class="sxs-lookup"><span data-stu-id="f1912-103">Update userExperienceAnalyticsScoreHistory</span></span>

<span data-ttu-id="f1912-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1912-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1912-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1912-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1912-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1912-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1912-107">Обновление свойств объекта [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="f1912-107">Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1912-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1912-108">Prerequisites</span></span>
<span data-ttu-id="f1912-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1912-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1912-111">Permission type</span></span>|<span data-ttu-id="f1912-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1912-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1912-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1912-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1912-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1912-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1912-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1912-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1912-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1912-116">Not supported.</span></span>|
|<span data-ttu-id="f1912-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f1912-117">Application</span></span>|<span data-ttu-id="f1912-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1912-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1912-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1912-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f1912-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1912-120">Request headers</span></span>
|<span data-ttu-id="f1912-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1912-121">Header</span></span>|<span data-ttu-id="f1912-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1912-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1912-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1912-123">Authorization</span></span>|<span data-ttu-id="f1912-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1912-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1912-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1912-125">Accept</span></span>|<span data-ttu-id="f1912-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1912-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1912-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1912-127">Request body</span></span>
<span data-ttu-id="f1912-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1912-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object.</span></span>

<span data-ttu-id="f1912-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span><span class="sxs-lookup"><span data-stu-id="f1912-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).</span></span>

|<span data-ttu-id="f1912-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1912-130">Property</span></span>|<span data-ttu-id="f1912-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1912-131">Type</span></span>|<span data-ttu-id="f1912-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1912-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1912-133">id</span><span class="sxs-lookup"><span data-stu-id="f1912-133">id</span></span>|<span data-ttu-id="f1912-134">String</span><span class="sxs-lookup"><span data-stu-id="f1912-134">String</span></span>|<span data-ttu-id="f1912-135">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1912-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="f1912-136">стартупдатетиме</span><span class="sxs-lookup"><span data-stu-id="f1912-136">startupDateTime</span></span>|<span data-ttu-id="f1912-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1912-137">DateTimeOffset</span></span>|<span data-ttu-id="f1912-138">Дата и время запуска устройства Analytics Device Experience.</span><span class="sxs-lookup"><span data-stu-id="f1912-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="f1912-139">стартупскоре</span><span class="sxs-lookup"><span data-stu-id="f1912-139">startupScore</span></span>|<span data-ttu-id="f1912-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f1912-140">Int32</span></span>|<span data-ttu-id="f1912-141">Оценка запуска устройства Analytics для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1912-141">User experience analytics device startup score.</span></span> <span data-ttu-id="f1912-142">Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.</span><span class="sxs-lookup"><span data-stu-id="f1912-142">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="f1912-143">коребутскоре</span><span class="sxs-lookup"><span data-stu-id="f1912-143">coreBootScore</span></span>|<span data-ttu-id="f1912-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f1912-144">Int32</span></span>|<span data-ttu-id="f1912-145">Оценка загрузки ядра устройств для службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1912-145">The user experience analytics device core boot score.</span></span> <span data-ttu-id="f1912-146">Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.</span><span class="sxs-lookup"><span data-stu-id="f1912-146">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="f1912-147">коресигнинскоре</span><span class="sxs-lookup"><span data-stu-id="f1912-147">coreSigninScore</span></span>|<span data-ttu-id="f1912-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f1912-148">Int32</span></span>|<span data-ttu-id="f1912-149">Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="f1912-149">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="f1912-150">Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.</span><span class="sxs-lookup"><span data-stu-id="f1912-150">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="f1912-151">рекоммендедсофтварескоре</span><span class="sxs-lookup"><span data-stu-id="f1912-151">recommendedSoftwareScore</span></span>|<span data-ttu-id="f1912-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f1912-152">Int32</span></span>|<span data-ttu-id="f1912-153">Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="f1912-153">The User experience analytics device core sign-in score.</span></span> <span data-ttu-id="f1912-154">Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель.</span><span class="sxs-lookup"><span data-stu-id="f1912-154">Score will be in the range 0-100, 100 is the ideal score.</span></span>|
|<span data-ttu-id="f1912-155">рестартскоре</span><span class="sxs-lookup"><span data-stu-id="f1912-155">restartScore</span></span>|<span data-ttu-id="f1912-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f1912-156">Int32</span></span>|<span data-ttu-id="f1912-157">Оценка перезапуска.</span><span class="sxs-lookup"><span data-stu-id="f1912-157">Restart score.</span></span> <span data-ttu-id="f1912-158">Показатель будет находиться в диапазоне 0-100, 100 — идеальный показатель, 0 указывает на чрезмерные перегрузки.</span><span class="sxs-lookup"><span data-stu-id="f1912-158">Score will be in the range 0-100, 100 is the ideal score, 0 indicates excessive restarts.</span></span> <span data-ttu-id="f1912-159">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="f1912-159">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="f1912-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1912-160">Response</span></span>
<span data-ttu-id="f1912-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксскорехистори](../resources/intune-devices-userexperienceanalyticsscorehistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1912-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1912-162">Пример</span><span class="sxs-lookup"><span data-stu-id="f1912-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1912-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1912-163">Request</span></span>
<span data-ttu-id="f1912-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1912-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1912-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1912-165">Response</span></span>
<span data-ttu-id="f1912-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1912-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



