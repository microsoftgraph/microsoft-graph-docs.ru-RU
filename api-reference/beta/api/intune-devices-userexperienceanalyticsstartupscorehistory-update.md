---
title: Обновление Усерекспериенцеаналитиксстартупскорехистори
description: Обновление свойств объекта Усерекспериенцеаналитиксстартупскорехистори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4645c627a54f0476c0928bb5bfd2267a04741fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467958"
---
# <a name="update-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="51e56-103">Обновление Усерекспериенцеаналитиксстартупскорехистори</span><span class="sxs-lookup"><span data-stu-id="51e56-103">Update userExperienceAnalyticsStartupScoreHistory</span></span>

<span data-ttu-id="51e56-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="51e56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51e56-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51e56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51e56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51e56-107">Обновление свойств объекта [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="51e56-107">Update the properties of a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51e56-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51e56-108">Prerequisites</span></span>
<span data-ttu-id="51e56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51e56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51e56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51e56-111">Permission type</span></span>|<span data-ttu-id="51e56-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51e56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51e56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51e56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51e56-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e56-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="51e56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51e56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51e56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51e56-116">Not supported.</span></span>|
|<span data-ttu-id="51e56-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51e56-117">Application</span></span>|<span data-ttu-id="51e56-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e56-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51e56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51e56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="51e56-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51e56-120">Request headers</span></span>
|<span data-ttu-id="51e56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51e56-121">Header</span></span>|<span data-ttu-id="51e56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51e56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51e56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e56-123">Authorization</span></span>|<span data-ttu-id="51e56-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51e56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51e56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51e56-125">Accept</span></span>|<span data-ttu-id="51e56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51e56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51e56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51e56-127">Request body</span></span>
<span data-ttu-id="51e56-128">В тексте запроса добавьте представление объекта [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51e56-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

<span data-ttu-id="51e56-129">В следующей таблице приведены свойства, необходимые при создании [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).</span><span class="sxs-lookup"><span data-stu-id="51e56-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).</span></span>

|<span data-ttu-id="51e56-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="51e56-130">Property</span></span>|<span data-ttu-id="51e56-131">Тип</span><span class="sxs-lookup"><span data-stu-id="51e56-131">Type</span></span>|<span data-ttu-id="51e56-132">Описание</span><span class="sxs-lookup"><span data-stu-id="51e56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e56-133">id</span><span class="sxs-lookup"><span data-stu-id="51e56-133">id</span></span>|<span data-ttu-id="51e56-134">String</span><span class="sxs-lookup"><span data-stu-id="51e56-134">String</span></span>|<span data-ttu-id="51e56-135">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="51e56-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="51e56-136">стартупдатетиме</span><span class="sxs-lookup"><span data-stu-id="51e56-136">startupDateTime</span></span>|<span data-ttu-id="51e56-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51e56-137">DateTimeOffset</span></span>|<span data-ttu-id="51e56-138">Дата и время запуска устройства Analytics Device Experience.</span><span class="sxs-lookup"><span data-stu-id="51e56-138">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="51e56-139">стартупскоре</span><span class="sxs-lookup"><span data-stu-id="51e56-139">startupScore</span></span>|<span data-ttu-id="51e56-140">Int32</span><span class="sxs-lookup"><span data-stu-id="51e56-140">Int32</span></span>|<span data-ttu-id="51e56-141">Оценка запуска устройства Analytics для пользователя.</span><span class="sxs-lookup"><span data-stu-id="51e56-141">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="51e56-142">коребутскоре</span><span class="sxs-lookup"><span data-stu-id="51e56-142">coreBootScore</span></span>|<span data-ttu-id="51e56-143">Int32</span><span class="sxs-lookup"><span data-stu-id="51e56-143">Int32</span></span>|<span data-ttu-id="51e56-144">Оценка загрузки ядра устройств для службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="51e56-144">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="51e56-145">коресигнинскоре</span><span class="sxs-lookup"><span data-stu-id="51e56-145">coreSigninScore</span></span>|<span data-ttu-id="51e56-146">Int32</span><span class="sxs-lookup"><span data-stu-id="51e56-146">Int32</span></span>|<span data-ttu-id="51e56-147">Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="51e56-147">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="51e56-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e56-148">Response</span></span>
<span data-ttu-id="51e56-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51e56-149">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e56-150">Пример</span><span class="sxs-lookup"><span data-stu-id="51e56-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="51e56-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="51e56-151">Request</span></span>
<span data-ttu-id="51e56-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51e56-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory/{userExperienceAnalyticsStartupScoreHistoryId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15
}
```

### <a name="response"></a><span data-ttu-id="51e56-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="51e56-153">Response</span></span>
<span data-ttu-id="51e56-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51e56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "52efee0b-ee0b-52ef-0bee-ef520beeef52",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15
}
```





