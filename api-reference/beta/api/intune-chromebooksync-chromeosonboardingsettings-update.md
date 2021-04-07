---
title: Обновление chromeOSOnboardingSettings
description: Обновление свойств объекта chromeOSOnboardingSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67d1d84e51500a5b3ade7dda7af2bdf4bdeb71f9
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611819"
---
# <a name="update-chromeosonboardingsettings"></a><span data-ttu-id="3c241-103">Обновление chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="3c241-103">Update chromeOSOnboardingSettings</span></span>

<span data-ttu-id="3c241-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c241-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c241-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c241-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c241-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c241-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c241-107">Обновление свойств объекта [chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3c241-107">Update the properties of a [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c241-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3c241-108">Prerequisites</span></span>
<span data-ttu-id="3c241-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c241-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c241-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c241-111">Permission type</span></span>|<span data-ttu-id="3c241-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c241-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c241-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c241-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c241-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c241-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c241-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c241-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c241-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c241-116">Not supported.</span></span>|
|<span data-ttu-id="3c241-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3c241-117">Application</span></span>|<span data-ttu-id="3c241-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c241-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c241-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c241-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/chromeOSOnboardingSettings/{chromeOSOnboardingSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="3c241-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3c241-120">Request headers</span></span>
|<span data-ttu-id="3c241-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c241-121">Header</span></span>|<span data-ttu-id="3c241-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c241-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c241-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c241-123">Authorization</span></span>|<span data-ttu-id="3c241-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c241-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c241-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c241-125">Accept</span></span>|<span data-ttu-id="3c241-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c241-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c241-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c241-127">Request body</span></span>
<span data-ttu-id="3c241-128">В корпусе запроса поставляем представление JSON для [объекта chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3c241-128">In the request body, supply a JSON representation for the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

<span data-ttu-id="3c241-129">В следующей таблице показаны свойства, необходимые при создании [chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3c241-129">The following table shows the properties that are required when you create the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md).</span></span>

|<span data-ttu-id="3c241-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c241-130">Property</span></span>|<span data-ttu-id="3c241-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3c241-131">Type</span></span>|<span data-ttu-id="3c241-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3c241-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c241-133">id</span><span class="sxs-lookup"><span data-stu-id="3c241-133">id</span></span>|<span data-ttu-id="3c241-134">String</span><span class="sxs-lookup"><span data-stu-id="3c241-134">String</span></span>|<span data-ttu-id="3c241-135">Id ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="3c241-135">The ChromebookTenant's Id</span></span>|
|<span data-ttu-id="3c241-136">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3c241-136">ownerUserPrincipalName</span></span>|<span data-ttu-id="3c241-137">String</span><span class="sxs-lookup"><span data-stu-id="3c241-137">String</span></span>|<span data-ttu-id="3c241-138">OwnerUserPrincipalName ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="3c241-138">The ChromebookTenant's OwnerUserPrincipalName</span></span>|
|<span data-ttu-id="3c241-139">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="3c241-139">onboardingStatus</span></span>|[<span data-ttu-id="3c241-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="3c241-140">onboardingStatus</span></span>](../resources/intune-chromebooksync-onboardingstatus.md)|<span data-ttu-id="3c241-141">OnboardingStatus ChromebookTenant.</span><span class="sxs-lookup"><span data-stu-id="3c241-141">The ChromebookTenant's OnboardingStatus.</span></span> <span data-ttu-id="3c241-142">Возможные значения: `unknown`, `inprogress`, `onboarded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3c241-142">Possible values are: `unknown`, `inprogress`, `onboarded`, `failed`.</span></span>|
|<span data-ttu-id="3c241-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c241-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3c241-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c241-144">DateTimeOffset</span></span>|<span data-ttu-id="3c241-145">LastModifiedDateTime ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="3c241-145">The ChromebookTenant's LastModifiedDateTime</span></span>|
|<span data-ttu-id="3c241-146">lastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3c241-146">lastDirectorySyncDateTime</span></span>|<span data-ttu-id="3c241-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c241-147">DateTimeOffset</span></span>|<span data-ttu-id="3c241-148">LastDirectorySyncDateTime в ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="3c241-148">The ChromebookTenant's LastDirectorySyncDateTime</span></span>|



## <a name="response"></a><span data-ttu-id="3c241-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c241-149">Response</span></span>
<span data-ttu-id="3c241-150">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3c241-150">If successful, this method returns a `200 OK` response code and an updated [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c241-151">Пример</span><span class="sxs-lookup"><span data-stu-id="3c241-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c241-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c241-152">Request</span></span>
<span data-ttu-id="3c241-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c241-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings/{chromeOSOnboardingSettingsId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3c241-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c241-154">Response</span></span>
<span data-ttu-id="3c241-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c241-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "0344255d-255d-0344-5d25-44035d254403",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```




