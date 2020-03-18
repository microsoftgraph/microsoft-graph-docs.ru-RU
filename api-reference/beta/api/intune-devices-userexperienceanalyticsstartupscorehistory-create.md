---
title: Создание Усерекспериенцеаналитиксстартупскорехистори
description: Создание нового объекта Усерекспериенцеаналитиксстартупскорехистори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83f83c797e7a2a1bf5852453572f1e94b84d6d93
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813777"
---
# <a name="create-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="30b32-103">Создание Усерекспериенцеаналитиксстартупскорехистори</span><span class="sxs-lookup"><span data-stu-id="30b32-103">Create userExperienceAnalyticsStartupScoreHistory</span></span>

> <span data-ttu-id="30b32-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30b32-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30b32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30b32-106">Создание нового объекта [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="30b32-106">Create a new [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30b32-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30b32-107">Prerequisites</span></span>
<span data-ttu-id="30b32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b32-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30b32-110">Permission type</span></span>|<span data-ttu-id="30b32-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30b32-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30b32-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30b32-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30b32-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b32-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="30b32-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30b32-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30b32-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b32-115">Not supported.</span></span>|
|<span data-ttu-id="30b32-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="30b32-116">Application</span></span>|<span data-ttu-id="30b32-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b32-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30b32-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30b32-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="30b32-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30b32-119">Request headers</span></span>
|<span data-ttu-id="30b32-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30b32-120">Header</span></span>|<span data-ttu-id="30b32-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30b32-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30b32-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30b32-122">Authorization</span></span>|<span data-ttu-id="30b32-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30b32-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30b32-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30b32-124">Accept</span></span>|<span data-ttu-id="30b32-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30b32-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30b32-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30b32-126">Request body</span></span>
<span data-ttu-id="30b32-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксстартупскорехистори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30b32-127">In the request body, supply a JSON representation for the userExperienceAnalyticsStartupScoreHistory object.</span></span>

<span data-ttu-id="30b32-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксстартупскорехистори.</span><span class="sxs-lookup"><span data-stu-id="30b32-128">The following table shows the properties that are required when you create the userExperienceAnalyticsStartupScoreHistory.</span></span>

|<span data-ttu-id="30b32-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="30b32-129">Property</span></span>|<span data-ttu-id="30b32-130">Тип</span><span class="sxs-lookup"><span data-stu-id="30b32-130">Type</span></span>|<span data-ttu-id="30b32-131">Описание</span><span class="sxs-lookup"><span data-stu-id="30b32-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30b32-132">id</span><span class="sxs-lookup"><span data-stu-id="30b32-132">id</span></span>|<span data-ttu-id="30b32-133">String</span><span class="sxs-lookup"><span data-stu-id="30b32-133">String</span></span>|<span data-ttu-id="30b32-134">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="30b32-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="30b32-135">стартупдатетиме</span><span class="sxs-lookup"><span data-stu-id="30b32-135">startupDateTime</span></span>|<span data-ttu-id="30b32-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30b32-136">DateTimeOffset</span></span>|<span data-ttu-id="30b32-137">Дата и время запуска устройства Analytics Device Experience.</span><span class="sxs-lookup"><span data-stu-id="30b32-137">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="30b32-138">стартупскоре</span><span class="sxs-lookup"><span data-stu-id="30b32-138">startupScore</span></span>|<span data-ttu-id="30b32-139">Int32</span><span class="sxs-lookup"><span data-stu-id="30b32-139">Int32</span></span>|<span data-ttu-id="30b32-140">Оценка запуска устройства Analytics для пользователя.</span><span class="sxs-lookup"><span data-stu-id="30b32-140">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="30b32-141">коребутскоре</span><span class="sxs-lookup"><span data-stu-id="30b32-141">coreBootScore</span></span>|<span data-ttu-id="30b32-142">Int32</span><span class="sxs-lookup"><span data-stu-id="30b32-142">Int32</span></span>|<span data-ttu-id="30b32-143">Оценка загрузки ядра устройств для службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="30b32-143">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="30b32-144">коресигнинскоре</span><span class="sxs-lookup"><span data-stu-id="30b32-144">coreSigninScore</span></span>|<span data-ttu-id="30b32-145">Int32</span><span class="sxs-lookup"><span data-stu-id="30b32-145">Int32</span></span>|<span data-ttu-id="30b32-146">Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="30b32-146">The User experience analytics device core sign-in score.</span></span>|
|<span data-ttu-id="30b32-147">рекоммендедсофтварескоре</span><span class="sxs-lookup"><span data-stu-id="30b32-147">recommendedSoftwareScore</span></span>|<span data-ttu-id="30b32-148">Int32</span><span class="sxs-lookup"><span data-stu-id="30b32-148">Int32</span></span>|<span data-ttu-id="30b32-149">Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="30b32-149">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="30b32-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b32-150">Response</span></span>
<span data-ttu-id="30b32-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30b32-151">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30b32-152">Пример</span><span class="sxs-lookup"><span data-stu-id="30b32-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="30b32-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="30b32-153">Request</span></span>
<span data-ttu-id="30b32-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30b32-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8
}
```

### <a name="response"></a><span data-ttu-id="30b32-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b32-155">Response</span></span>
<span data-ttu-id="30b32-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30b32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "52efee0b-ee0b-52ef-0bee-ef520beeef52",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8
}
```




