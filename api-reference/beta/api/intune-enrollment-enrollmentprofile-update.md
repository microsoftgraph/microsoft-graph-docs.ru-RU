---
title: Обновление enrollmentProfile
description: Обновление свойства объекта enrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85cceaaaaa66822340539c38f6ab8ecde88eae1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400741"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="e89c6-103">Обновление enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e89c6-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="e89c6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e89c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e89c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e89c6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e89c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e89c6-107">Обновление свойства объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e89c6-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e89c6-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e89c6-108">Prerequisites</span></span>
<span data-ttu-id="e89c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e89c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e89c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e89c6-111">Permission type</span></span>|<span data-ttu-id="e89c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e89c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e89c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e89c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e89c6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e89c6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e89c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e89c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e89c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89c6-116">Not supported.</span></span>|
|<span data-ttu-id="e89c6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e89c6-117">Application</span></span>|<span data-ttu-id="e89c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e89c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e89c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e89c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="e89c6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e89c6-120">Request headers</span></span>
|<span data-ttu-id="e89c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e89c6-121">Header</span></span>|<span data-ttu-id="e89c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e89c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e89c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e89c6-123">Authorization</span></span>|<span data-ttu-id="e89c6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e89c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e89c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e89c6-125">Accept</span></span>|<span data-ttu-id="e89c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e89c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e89c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e89c6-127">Request body</span></span>
<span data-ttu-id="e89c6-128">В тексте запроса укажите представление JSON для объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e89c6-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="e89c6-129">В следующей таблице показаны свойства, которые необходимы для создания [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e89c6-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="e89c6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e89c6-130">Property</span></span>|<span data-ttu-id="e89c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e89c6-131">Type</span></span>|<span data-ttu-id="e89c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e89c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e89c6-133">id</span><span class="sxs-lookup"><span data-stu-id="e89c6-133">id</span></span>|<span data-ttu-id="e89c6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e89c6-134">String</span></span>|<span data-ttu-id="e89c6-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="e89c6-135">The GUID for the object</span></span>|
|<span data-ttu-id="e89c6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e89c6-136">displayName</span></span>|<span data-ttu-id="e89c6-137">String</span><span class="sxs-lookup"><span data-stu-id="e89c6-137">String</span></span>|<span data-ttu-id="e89c6-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="e89c6-138">Name of the profile</span></span>|
|<span data-ttu-id="e89c6-139">description</span><span class="sxs-lookup"><span data-stu-id="e89c6-139">description</span></span>|<span data-ttu-id="e89c6-140">String</span><span class="sxs-lookup"><span data-stu-id="e89c6-140">String</span></span>|<span data-ttu-id="e89c6-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="e89c6-141">Description of the profile</span></span>|
|<span data-ttu-id="e89c6-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e89c6-142">requiresUserAuthentication</span></span>|<span data-ttu-id="e89c6-143">Логический</span><span class="sxs-lookup"><span data-stu-id="e89c6-143">Boolean</span></span>|<span data-ttu-id="e89c6-144">Указывает необходимость проверки подлинности пользователей в профиле</span><span class="sxs-lookup"><span data-stu-id="e89c6-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="e89c6-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e89c6-145">configurationEndpointUrl</span></span>|<span data-ttu-id="e89c6-146">String</span><span class="sxs-lookup"><span data-stu-id="e89c6-146">String</span></span>|<span data-ttu-id="e89c6-147">URL-адрес конечной точки конфигурации для подачи заявок</span><span class="sxs-lookup"><span data-stu-id="e89c6-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="e89c6-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e89c6-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e89c6-149">Логический</span><span class="sxs-lookup"><span data-stu-id="e89c6-149">Boolean</span></span>|<span data-ttu-id="e89c6-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="e89c6-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="e89c6-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="e89c6-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="e89c6-152">Логический</span><span class="sxs-lookup"><span data-stu-id="e89c6-152">Boolean</span></span>|<span data-ttu-id="e89c6-153">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки</span><span class="sxs-lookup"><span data-stu-id="e89c6-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="e89c6-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89c6-154">Response</span></span>
<span data-ttu-id="e89c6-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e89c6-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e89c6-156">Пример</span><span class="sxs-lookup"><span data-stu-id="e89c6-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="e89c6-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="e89c6-157">Request</span></span>
<span data-ttu-id="e89c6-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e89c6-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e89c6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e89c6-159">Response</span></span>
<span data-ttu-id="e89c6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e89c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




