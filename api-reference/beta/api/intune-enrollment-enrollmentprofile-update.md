---
title: Обновление объекта enrollmentprofile
description: Обновление свойств объекта объекта enrollmentprofile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5a02d72a277cb973d92ba2d96bdecf1978f5e34
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185149"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="9a5b4-103">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="9a5b4-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="9a5b4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a5b4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a5b4-106">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9a5b4-106">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a5b4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9a5b4-107">Prerequisites</span></span>
<span data-ttu-id="9a5b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a5b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a5b4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a5b4-110">Permission type</span></span>|<span data-ttu-id="9a5b4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a5b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a5b4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a5b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a5b4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a5b4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9a5b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a5b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a5b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-115">Not supported.</span></span>|
|<span data-ttu-id="9a5b4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a5b4-116">Application</span></span>|<span data-ttu-id="9a5b4-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a5b4-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a5b4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a5b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="9a5b4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a5b4-119">Request headers</span></span>
|<span data-ttu-id="9a5b4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a5b4-120">Header</span></span>|<span data-ttu-id="9a5b4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9a5b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a5b4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a5b4-122">Authorization</span></span>|<span data-ttu-id="9a5b4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a5b4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9a5b4-124">Accept</span></span>|<span data-ttu-id="9a5b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a5b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a5b4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a5b4-126">Request body</span></span>
<span data-ttu-id="9a5b4-127">В тексте запроса добавьте представление объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-127">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="9a5b4-128">В следующей таблице приведены свойства, необходимые при создании [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9a5b4-128">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="9a5b4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a5b4-129">Property</span></span>|<span data-ttu-id="9a5b4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9a5b4-130">Type</span></span>|<span data-ttu-id="9a5b4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9a5b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a5b4-132">id</span><span class="sxs-lookup"><span data-stu-id="9a5b4-132">id</span></span>|<span data-ttu-id="9a5b4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9a5b4-133">String</span></span>|<span data-ttu-id="9a5b4-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="9a5b4-134">The GUID for the object</span></span>|
|<span data-ttu-id="9a5b4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9a5b4-135">displayName</span></span>|<span data-ttu-id="9a5b4-136">Строка</span><span class="sxs-lookup"><span data-stu-id="9a5b4-136">String</span></span>|<span data-ttu-id="9a5b4-137">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="9a5b4-137">Name of the profile</span></span>|
|<span data-ttu-id="9a5b4-138">description</span><span class="sxs-lookup"><span data-stu-id="9a5b4-138">description</span></span>|<span data-ttu-id="9a5b4-139">String</span><span class="sxs-lookup"><span data-stu-id="9a5b4-139">String</span></span>|<span data-ttu-id="9a5b4-140">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="9a5b4-140">Description of the profile</span></span>|
|<span data-ttu-id="9a5b4-141">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="9a5b4-141">requiresUserAuthentication</span></span>|<span data-ttu-id="9a5b4-142">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-142">Boolean</span></span>|<span data-ttu-id="9a5b4-143">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="9a5b4-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="9a5b4-144">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="9a5b4-144">configurationEndpointUrl</span></span>|<span data-ttu-id="9a5b4-145">String.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-145">String</span></span>|<span data-ttu-id="9a5b4-146">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="9a5b4-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="9a5b4-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="9a5b4-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="9a5b4-148">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-148">Boolean</span></span>|<span data-ttu-id="9a5b4-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="9a5b4-150">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="9a5b4-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="9a5b4-151">Boolean.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-151">Boolean</span></span>|<span data-ttu-id="9a5b4-152">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="9a5b4-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="9a5b4-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a5b4-153">Response</span></span>
<span data-ttu-id="9a5b4-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-154">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a5b4-155">Пример</span><span class="sxs-lookup"><span data-stu-id="9a5b4-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a5b4-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a5b4-156">Request</span></span>
<span data-ttu-id="9a5b4-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a5b4-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a5b4-158">Response</span></span>
<span data-ttu-id="9a5b4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a5b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




