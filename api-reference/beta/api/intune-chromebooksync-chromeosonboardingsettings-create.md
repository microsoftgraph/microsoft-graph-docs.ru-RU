---
title: Создание chromeOSOnboardingSettings
description: Создайте новый объект chromeOSOnboardingSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a359b9bd0f638e147af8119ee7ca07a27db0c2e8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665975"
---
# <a name="create-chromeosonboardingsettings"></a><span data-ttu-id="06562-103">Создание chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="06562-103">Create chromeOSOnboardingSettings</span></span>

<span data-ttu-id="06562-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06562-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06562-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06562-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06562-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06562-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06562-107">Создайте новый [объект chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)</span><span class="sxs-lookup"><span data-stu-id="06562-107">Create a new [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06562-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06562-108">Prerequisites</span></span>
<span data-ttu-id="06562-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06562-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06562-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06562-111">Permission type</span></span>|<span data-ttu-id="06562-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06562-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06562-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06562-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06562-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06562-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06562-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06562-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06562-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06562-116">Not supported.</span></span>|
|<span data-ttu-id="06562-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="06562-117">Application</span></span>|<span data-ttu-id="06562-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06562-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06562-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06562-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="06562-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="06562-120">Request headers</span></span>
|<span data-ttu-id="06562-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06562-121">Header</span></span>|<span data-ttu-id="06562-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06562-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06562-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06562-123">Authorization</span></span>|<span data-ttu-id="06562-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06562-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06562-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06562-125">Accept</span></span>|<span data-ttu-id="06562-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06562-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06562-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06562-127">Request body</span></span>
<span data-ttu-id="06562-128">В корпусе запроса поставляем представление JSON для объекта chromeOSOnboardingSettings.</span><span class="sxs-lookup"><span data-stu-id="06562-128">In the request body, supply a JSON representation for the chromeOSOnboardingSettings object.</span></span>

<span data-ttu-id="06562-129">В следующей таблице показаны свойства, необходимые при создании chromeOSOnboardingSettings.</span><span class="sxs-lookup"><span data-stu-id="06562-129">The following table shows the properties that are required when you create the chromeOSOnboardingSettings.</span></span>

|<span data-ttu-id="06562-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="06562-130">Property</span></span>|<span data-ttu-id="06562-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06562-131">Type</span></span>|<span data-ttu-id="06562-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06562-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06562-133">id</span><span class="sxs-lookup"><span data-stu-id="06562-133">id</span></span>|<span data-ttu-id="06562-134">Строка</span><span class="sxs-lookup"><span data-stu-id="06562-134">String</span></span>|<span data-ttu-id="06562-135">Id ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="06562-135">The ChromebookTenant's Id</span></span>|
|<span data-ttu-id="06562-136">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06562-136">ownerUserPrincipalName</span></span>|<span data-ttu-id="06562-137">String</span><span class="sxs-lookup"><span data-stu-id="06562-137">String</span></span>|<span data-ttu-id="06562-138">OwnerUserPrincipalName ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="06562-138">The ChromebookTenant's OwnerUserPrincipalName</span></span>|
|<span data-ttu-id="06562-139">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="06562-139">onboardingStatus</span></span>|[<span data-ttu-id="06562-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="06562-140">onboardingStatus</span></span>](../resources/intune-chromebooksync-onboardingstatus.md)|<span data-ttu-id="06562-141">OnboardingStatus ChromebookTenant.</span><span class="sxs-lookup"><span data-stu-id="06562-141">The ChromebookTenant's OnboardingStatus.</span></span> <span data-ttu-id="06562-142">Возможные значения: `unknown`, `inprogress`, `onboarded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="06562-142">Possible values are: `unknown`, `inprogress`, `onboarded`, `failed`.</span></span>|
|<span data-ttu-id="06562-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06562-143">lastModifiedDateTime</span></span>|<span data-ttu-id="06562-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06562-144">DateTimeOffset</span></span>|<span data-ttu-id="06562-145">LastModifiedDateTime ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="06562-145">The ChromebookTenant's LastModifiedDateTime</span></span>|
|<span data-ttu-id="06562-146">lastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="06562-146">lastDirectorySyncDateTime</span></span>|<span data-ttu-id="06562-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06562-147">DateTimeOffset</span></span>|<span data-ttu-id="06562-148">LastDirectorySyncDateTime в ChromebookTenant</span><span class="sxs-lookup"><span data-stu-id="06562-148">The ChromebookTenant's LastDirectorySyncDateTime</span></span>|



## <a name="response"></a><span data-ttu-id="06562-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="06562-149">Response</span></span>
<span data-ttu-id="06562-150">В случае успеха этот метод возвращает код отклика и `201 Created` [объект chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="06562-150">If successful, this method returns a `201 Created` response code and a [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06562-151">Пример</span><span class="sxs-lookup"><span data-stu-id="06562-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="06562-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="06562-152">Request</span></span>
<span data-ttu-id="06562-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06562-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "onboardingStatus": "inprogress",
  "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
}
```

### <a name="response"></a><span data-ttu-id="06562-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="06562-154">Response</span></span>
<span data-ttu-id="06562-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06562-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




