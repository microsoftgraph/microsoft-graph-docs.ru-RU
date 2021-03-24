---
title: Обновление enrollmentProfile
description: Обновление свойств объекта enrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53031ccf2db85727f35cf8ef376682a1944d3a29
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126229"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="2a360-103">Обновление enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="2a360-103">Update enrollmentProfile</span></span>

<span data-ttu-id="2a360-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a360-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a360-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a360-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a360-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a360-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a360-107">Обновление свойств объекта [enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2a360-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a360-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2a360-108">Prerequisites</span></span>
<span data-ttu-id="2a360-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a360-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a360-111">Permission type</span></span>|<span data-ttu-id="2a360-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a360-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a360-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a360-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a360-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a360-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a360-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a360-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a360-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a360-116">Not supported.</span></span>|
|<span data-ttu-id="2a360-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a360-117">Application</span></span>|<span data-ttu-id="2a360-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a360-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a360-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a360-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="2a360-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a360-120">Request headers</span></span>
|<span data-ttu-id="2a360-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a360-121">Header</span></span>|<span data-ttu-id="2a360-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2a360-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a360-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a360-123">Authorization</span></span>|<span data-ttu-id="2a360-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a360-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a360-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2a360-125">Accept</span></span>|<span data-ttu-id="2a360-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a360-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a360-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a360-127">Request body</span></span>
<span data-ttu-id="2a360-128">В теле запроса поставляем представление JSON для объекта [enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2a360-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="2a360-129">В следующей таблице показаны свойства, необходимые при создании [enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2a360-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="2a360-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a360-130">Property</span></span>|<span data-ttu-id="2a360-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2a360-131">Type</span></span>|<span data-ttu-id="2a360-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2a360-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a360-133">id</span><span class="sxs-lookup"><span data-stu-id="2a360-133">id</span></span>|<span data-ttu-id="2a360-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2a360-134">String</span></span>|<span data-ttu-id="2a360-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="2a360-135">The GUID for the object</span></span>|
|<span data-ttu-id="2a360-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2a360-136">displayName</span></span>|<span data-ttu-id="2a360-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2a360-137">String</span></span>|<span data-ttu-id="2a360-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="2a360-138">Name of the profile</span></span>|
|<span data-ttu-id="2a360-139">description</span><span class="sxs-lookup"><span data-stu-id="2a360-139">description</span></span>|<span data-ttu-id="2a360-140">Строка</span><span class="sxs-lookup"><span data-stu-id="2a360-140">String</span></span>|<span data-ttu-id="2a360-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="2a360-141">Description of the profile</span></span>|
|<span data-ttu-id="2a360-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="2a360-142">requiresUserAuthentication</span></span>|<span data-ttu-id="2a360-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a360-143">Boolean</span></span>|<span data-ttu-id="2a360-144">Указывает, требует ли профиль проверки подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="2a360-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="2a360-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="2a360-145">configurationEndpointUrl</span></span>|<span data-ttu-id="2a360-146">Строка</span><span class="sxs-lookup"><span data-stu-id="2a360-146">String</span></span>|<span data-ttu-id="2a360-147">URL-адрес конечной точки конфигурации для регистрации</span><span class="sxs-lookup"><span data-stu-id="2a360-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="2a360-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2a360-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="2a360-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a360-149">Boolean</span></span>|<span data-ttu-id="2a360-150">Указывает на проверку подлинности с помощью помощника установки Apple вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="2a360-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="2a360-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="2a360-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="2a360-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a360-152">Boolean</span></span>|<span data-ttu-id="2a360-153">Указывает, что портал компании необходим для устройств, зарегистрированных помощником установки</span><span class="sxs-lookup"><span data-stu-id="2a360-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="2a360-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a360-154">Response</span></span>
<span data-ttu-id="2a360-155">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2a360-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a360-156">Пример</span><span class="sxs-lookup"><span data-stu-id="2a360-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a360-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a360-157">Request</span></span>
<span data-ttu-id="2a360-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a360-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 370

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

### <a name="response"></a><span data-ttu-id="2a360-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a360-159">Response</span></span>
<span data-ttu-id="2a360-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a360-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




