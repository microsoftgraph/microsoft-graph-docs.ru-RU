---
title: Создание enrollmentProfile
description: Создание нового объекта enrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a7bb3fb49b57f38ad938f7d43f28f4ece3fda92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414769"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="42cad-103">Создание enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="42cad-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="42cad-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42cad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42cad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42cad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42cad-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42cad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42cad-107">Создание нового объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="42cad-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42cad-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="42cad-108">Prerequisites</span></span>
<span data-ttu-id="42cad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42cad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42cad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42cad-111">Permission type</span></span>|<span data-ttu-id="42cad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42cad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42cad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42cad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42cad-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42cad-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42cad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42cad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42cad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42cad-116">Not supported.</span></span>|
|<span data-ttu-id="42cad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42cad-117">Application</span></span>|<span data-ttu-id="42cad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42cad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42cad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42cad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="42cad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42cad-120">Request headers</span></span>
|<span data-ttu-id="42cad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42cad-121">Header</span></span>|<span data-ttu-id="42cad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42cad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42cad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42cad-123">Authorization</span></span>|<span data-ttu-id="42cad-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42cad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42cad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42cad-125">Accept</span></span>|<span data-ttu-id="42cad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42cad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42cad-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42cad-127">Request body</span></span>
<span data-ttu-id="42cad-128">В тексте запроса укажите представление JSON для объекта enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="42cad-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="42cad-129">В следующей таблице показаны свойства, которые необходимы для создания enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="42cad-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="42cad-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42cad-130">Property</span></span>|<span data-ttu-id="42cad-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42cad-131">Type</span></span>|<span data-ttu-id="42cad-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42cad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42cad-133">id</span><span class="sxs-lookup"><span data-stu-id="42cad-133">id</span></span>|<span data-ttu-id="42cad-134">Строка</span><span class="sxs-lookup"><span data-stu-id="42cad-134">String</span></span>|<span data-ttu-id="42cad-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="42cad-135">The GUID for the object</span></span>|
|<span data-ttu-id="42cad-136">displayName</span><span class="sxs-lookup"><span data-stu-id="42cad-136">displayName</span></span>|<span data-ttu-id="42cad-137">String</span><span class="sxs-lookup"><span data-stu-id="42cad-137">String</span></span>|<span data-ttu-id="42cad-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="42cad-138">Name of the profile</span></span>|
|<span data-ttu-id="42cad-139">description</span><span class="sxs-lookup"><span data-stu-id="42cad-139">description</span></span>|<span data-ttu-id="42cad-140">String</span><span class="sxs-lookup"><span data-stu-id="42cad-140">String</span></span>|<span data-ttu-id="42cad-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="42cad-141">Description of the profile</span></span>|
|<span data-ttu-id="42cad-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="42cad-142">requiresUserAuthentication</span></span>|<span data-ttu-id="42cad-143">Логический</span><span class="sxs-lookup"><span data-stu-id="42cad-143">Boolean</span></span>|<span data-ttu-id="42cad-144">Указывает необходимость проверки подлинности пользователей в профиле</span><span class="sxs-lookup"><span data-stu-id="42cad-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="42cad-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="42cad-145">configurationEndpointUrl</span></span>|<span data-ttu-id="42cad-146">String</span><span class="sxs-lookup"><span data-stu-id="42cad-146">String</span></span>|<span data-ttu-id="42cad-147">URL-адрес конечной точки конфигурации для подачи заявок</span><span class="sxs-lookup"><span data-stu-id="42cad-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="42cad-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="42cad-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="42cad-149">Логический</span><span class="sxs-lookup"><span data-stu-id="42cad-149">Boolean</span></span>|<span data-ttu-id="42cad-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="42cad-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="42cad-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="42cad-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="42cad-152">Логический</span><span class="sxs-lookup"><span data-stu-id="42cad-152">Boolean</span></span>|<span data-ttu-id="42cad-153">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки</span><span class="sxs-lookup"><span data-stu-id="42cad-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="42cad-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="42cad-154">Response</span></span>
<span data-ttu-id="42cad-155">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42cad-155">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42cad-156">Пример</span><span class="sxs-lookup"><span data-stu-id="42cad-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="42cad-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="42cad-157">Request</span></span>
<span data-ttu-id="42cad-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42cad-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="42cad-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="42cad-159">Response</span></span>
<span data-ttu-id="42cad-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42cad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




