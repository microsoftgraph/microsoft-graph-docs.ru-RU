---
title: Обновление объекта enrollmentprofile
description: Обновление свойств объекта объекта enrollmentprofile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc4bb4ca29ea3d63a9038b014aaffbcb7718b16b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450035"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="64f93-103">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="64f93-103">Update enrollmentProfile</span></span>

<span data-ttu-id="64f93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64f93-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64f93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f93-107">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="64f93-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64f93-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="64f93-108">Prerequisites</span></span>
<span data-ttu-id="64f93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64f93-111">Permission type</span></span>|<span data-ttu-id="64f93-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64f93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64f93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64f93-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64f93-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="64f93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64f93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f93-116">Not supported.</span></span>|
|<span data-ttu-id="64f93-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64f93-117">Application</span></span>|<span data-ttu-id="64f93-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64f93-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64f93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="64f93-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64f93-120">Request headers</span></span>
|<span data-ttu-id="64f93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64f93-121">Header</span></span>|<span data-ttu-id="64f93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64f93-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64f93-123">Authorization</span></span>|<span data-ttu-id="64f93-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64f93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64f93-125">Accept</span></span>|<span data-ttu-id="64f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f93-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64f93-127">Request body</span></span>
<span data-ttu-id="64f93-128">В тексте запроса добавьте представление объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64f93-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="64f93-129">В следующей таблице приведены свойства, необходимые при создании [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="64f93-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="64f93-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64f93-130">Property</span></span>|<span data-ttu-id="64f93-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64f93-131">Type</span></span>|<span data-ttu-id="64f93-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64f93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f93-133">id</span><span class="sxs-lookup"><span data-stu-id="64f93-133">id</span></span>|<span data-ttu-id="64f93-134">Строка</span><span class="sxs-lookup"><span data-stu-id="64f93-134">String</span></span>|<span data-ttu-id="64f93-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="64f93-135">The GUID for the object</span></span>|
|<span data-ttu-id="64f93-136">displayName</span><span class="sxs-lookup"><span data-stu-id="64f93-136">displayName</span></span>|<span data-ttu-id="64f93-137">Строка</span><span class="sxs-lookup"><span data-stu-id="64f93-137">String</span></span>|<span data-ttu-id="64f93-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="64f93-138">Name of the profile</span></span>|
|<span data-ttu-id="64f93-139">description</span><span class="sxs-lookup"><span data-stu-id="64f93-139">description</span></span>|<span data-ttu-id="64f93-140">String</span><span class="sxs-lookup"><span data-stu-id="64f93-140">String</span></span>|<span data-ttu-id="64f93-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="64f93-141">Description of the profile</span></span>|
|<span data-ttu-id="64f93-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="64f93-142">requiresUserAuthentication</span></span>|<span data-ttu-id="64f93-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="64f93-143">Boolean</span></span>|<span data-ttu-id="64f93-144">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="64f93-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="64f93-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="64f93-145">configurationEndpointUrl</span></span>|<span data-ttu-id="64f93-146">String</span><span class="sxs-lookup"><span data-stu-id="64f93-146">String</span></span>|<span data-ttu-id="64f93-147">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="64f93-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="64f93-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="64f93-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="64f93-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="64f93-149">Boolean</span></span>|<span data-ttu-id="64f93-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="64f93-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="64f93-151">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="64f93-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="64f93-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="64f93-152">Boolean</span></span>|<span data-ttu-id="64f93-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="64f93-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="64f93-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="64f93-154">Response</span></span>
<span data-ttu-id="64f93-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64f93-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f93-156">Пример</span><span class="sxs-lookup"><span data-stu-id="64f93-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="64f93-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="64f93-157">Request</span></span>
<span data-ttu-id="64f93-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64f93-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64f93-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="64f93-159">Response</span></span>
<span data-ttu-id="64f93-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64f93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



