---
title: Создание Усерекспериенцеаналитиксстартупскорехистори
description: Создание нового объекта Усерекспериенцеаналитиксстартупскорехистори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ad264473e516889269e2b74abfa0e89a7ce534e
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161940"
---
# <a name="create-userexperienceanalyticsstartupscorehistory"></a><span data-ttu-id="39107-103">Создание Усерекспериенцеаналитиксстартупскорехистори</span><span class="sxs-lookup"><span data-stu-id="39107-103">Create userExperienceAnalyticsStartupScoreHistory</span></span>

> <span data-ttu-id="39107-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39107-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39107-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39107-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39107-106">Создание нового объекта [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .</span><span class="sxs-lookup"><span data-stu-id="39107-106">Create a new [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39107-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39107-107">Prerequisites</span></span>
<span data-ttu-id="39107-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39107-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39107-110">Permission type</span></span>|<span data-ttu-id="39107-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39107-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39107-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39107-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39107-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39107-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="39107-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39107-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39107-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39107-115">Not supported.</span></span>|
|<span data-ttu-id="39107-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39107-116">Application</span></span>|<span data-ttu-id="39107-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39107-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39107-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39107-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsStartupScoreHistory
```

## <a name="request-headers"></a><span data-ttu-id="39107-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="39107-119">Request headers</span></span>
|<span data-ttu-id="39107-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39107-120">Header</span></span>|<span data-ttu-id="39107-121">Значение</span><span class="sxs-lookup"><span data-stu-id="39107-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39107-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="39107-122">Authorization</span></span>|<span data-ttu-id="39107-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39107-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39107-124">Accept</span><span class="sxs-lookup"><span data-stu-id="39107-124">Accept</span></span>|<span data-ttu-id="39107-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39107-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39107-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39107-126">Request body</span></span>
<span data-ttu-id="39107-127">В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксстартупскорехистори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39107-127">In the request body, supply a JSON representation for the userExperienceAnalyticsStartupScoreHistory object.</span></span>

<span data-ttu-id="39107-128">В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксстартупскорехистори.</span><span class="sxs-lookup"><span data-stu-id="39107-128">The following table shows the properties that are required when you create the userExperienceAnalyticsStartupScoreHistory.</span></span>

|<span data-ttu-id="39107-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="39107-129">Property</span></span>|<span data-ttu-id="39107-130">Тип</span><span class="sxs-lookup"><span data-stu-id="39107-130">Type</span></span>|<span data-ttu-id="39107-131">Описание</span><span class="sxs-lookup"><span data-stu-id="39107-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39107-132">id</span><span class="sxs-lookup"><span data-stu-id="39107-132">id</span></span>|<span data-ttu-id="39107-133">String</span><span class="sxs-lookup"><span data-stu-id="39107-133">String</span></span>|<span data-ttu-id="39107-134">Уникальный идентификатор процесса запуска устройства аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="39107-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="39107-135">стартупдатетиме</span><span class="sxs-lookup"><span data-stu-id="39107-135">startupDateTime</span></span>|<span data-ttu-id="39107-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39107-136">DateTimeOffset</span></span>|<span data-ttu-id="39107-137">Дата и время запуска устройства Analytics Device Experience.</span><span class="sxs-lookup"><span data-stu-id="39107-137">The user experience analytics device startup date time.</span></span>|
|<span data-ttu-id="39107-138">стартупскоре</span><span class="sxs-lookup"><span data-stu-id="39107-138">startupScore</span></span>|<span data-ttu-id="39107-139">Int32</span><span class="sxs-lookup"><span data-stu-id="39107-139">Int32</span></span>|<span data-ttu-id="39107-140">Оценка запуска устройства Analytics для пользователя.</span><span class="sxs-lookup"><span data-stu-id="39107-140">User experience analytics device startup score.</span></span>|
|<span data-ttu-id="39107-141">коребутскоре</span><span class="sxs-lookup"><span data-stu-id="39107-141">coreBootScore</span></span>|<span data-ttu-id="39107-142">Int32</span><span class="sxs-lookup"><span data-stu-id="39107-142">Int32</span></span>|<span data-ttu-id="39107-143">Оценка загрузки ядра устройств для службы аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="39107-143">The user experience analytics device core boot score.</span></span>|
|<span data-ttu-id="39107-144">коресигнинскоре</span><span class="sxs-lookup"><span data-stu-id="39107-144">coreSigninScore</span></span>|<span data-ttu-id="39107-145">Int32</span><span class="sxs-lookup"><span data-stu-id="39107-145">Int32</span></span>|<span data-ttu-id="39107-146">Показатель для входа в систему для устройства аналитики с пользовательским интерфейсом.</span><span class="sxs-lookup"><span data-stu-id="39107-146">The User experience analytics device core sign-in score.</span></span>|



## <a name="response"></a><span data-ttu-id="39107-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="39107-147">Response</span></span>
<span data-ttu-id="39107-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксстартупскорехистори](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39107-148">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39107-149">Пример</span><span class="sxs-lookup"><span data-stu-id="39107-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="39107-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="39107-150">Request</span></span>
<span data-ttu-id="39107-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39107-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsStartupScoreHistory
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

### <a name="response"></a><span data-ttu-id="39107-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="39107-152">Response</span></span>
<span data-ttu-id="39107-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39107-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





