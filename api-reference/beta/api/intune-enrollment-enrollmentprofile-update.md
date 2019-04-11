---
title: Обновление объекта enrollmentprofile
description: Обновление свойств объекта объекта enrollmentprofile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 593c760b303ca87a3bc2ddc77571719379557562
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773828"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="77351-103">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="77351-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="77351-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77351-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77351-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77351-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77351-106">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="77351-106">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77351-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77351-107">Prerequisites</span></span>
<span data-ttu-id="77351-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77351-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77351-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77351-110">Permission type</span></span>|<span data-ttu-id="77351-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77351-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77351-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77351-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77351-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77351-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77351-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77351-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77351-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77351-115">Not supported.</span></span>|
|<span data-ttu-id="77351-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77351-116">Application</span></span>|<span data-ttu-id="77351-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77351-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77351-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77351-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="77351-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77351-119">Request headers</span></span>
|<span data-ttu-id="77351-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77351-120">Header</span></span>|<span data-ttu-id="77351-121">Значение</span><span class="sxs-lookup"><span data-stu-id="77351-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77351-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77351-122">Authorization</span></span>|<span data-ttu-id="77351-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77351-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77351-124">Accept</span><span class="sxs-lookup"><span data-stu-id="77351-124">Accept</span></span>|<span data-ttu-id="77351-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77351-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77351-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77351-126">Request body</span></span>
<span data-ttu-id="77351-127">В тексте запроса добавьте представление объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77351-127">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="77351-128">В следующей таблице приведены свойства, необходимые при создании [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="77351-128">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="77351-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="77351-129">Property</span></span>|<span data-ttu-id="77351-130">Тип</span><span class="sxs-lookup"><span data-stu-id="77351-130">Type</span></span>|<span data-ttu-id="77351-131">Описание</span><span class="sxs-lookup"><span data-stu-id="77351-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77351-132">id</span><span class="sxs-lookup"><span data-stu-id="77351-132">id</span></span>|<span data-ttu-id="77351-133">Строка</span><span class="sxs-lookup"><span data-stu-id="77351-133">String</span></span>|<span data-ttu-id="77351-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="77351-134">The GUID for the object</span></span>|
|<span data-ttu-id="77351-135">displayName</span><span class="sxs-lookup"><span data-stu-id="77351-135">displayName</span></span>|<span data-ttu-id="77351-136">String</span><span class="sxs-lookup"><span data-stu-id="77351-136">String</span></span>|<span data-ttu-id="77351-137">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="77351-137">Name of the profile</span></span>|
|<span data-ttu-id="77351-138">description</span><span class="sxs-lookup"><span data-stu-id="77351-138">description</span></span>|<span data-ttu-id="77351-139">String</span><span class="sxs-lookup"><span data-stu-id="77351-139">String</span></span>|<span data-ttu-id="77351-140">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="77351-140">Description of the profile</span></span>|
|<span data-ttu-id="77351-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="77351-141">requiresUserAuthentication</span></span>|<span data-ttu-id="77351-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="77351-142">Boolean</span></span>|<span data-ttu-id="77351-143">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="77351-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="77351-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="77351-144">configurationEndpointUrl</span></span>|<span data-ttu-id="77351-145">String</span><span class="sxs-lookup"><span data-stu-id="77351-145">String</span></span>|<span data-ttu-id="77351-146">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="77351-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="77351-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="77351-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="77351-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="77351-148">Boolean</span></span>|<span data-ttu-id="77351-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="77351-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="77351-150">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="77351-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="77351-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="77351-151">Boolean</span></span>|<span data-ttu-id="77351-152">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="77351-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="77351-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="77351-153">Response</span></span>
<span data-ttu-id="77351-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77351-154">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77351-155">Пример</span><span class="sxs-lookup"><span data-stu-id="77351-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="77351-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="77351-156">Request</span></span>
<span data-ttu-id="77351-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77351-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77351-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="77351-158">Response</span></span>
<span data-ttu-id="77351-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77351-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





