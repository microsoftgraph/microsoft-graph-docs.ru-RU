---
title: Создание объекта enrollmentprofile
description: Создание нового объекта объекта enrollmentprofile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f65bc4807d76f4532eb3eadbcf818d47279a1440
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693152"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="409f3-103">Создание объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="409f3-103">Create enrollmentProfile</span></span>

<span data-ttu-id="409f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="409f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="409f3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="409f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="409f3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="409f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="409f3-107">Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="409f3-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="409f3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="409f3-108">Prerequisites</span></span>
<span data-ttu-id="409f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="409f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="409f3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="409f3-111">Permission type</span></span>|<span data-ttu-id="409f3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="409f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="409f3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="409f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="409f3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="409f3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="409f3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="409f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="409f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="409f3-116">Not supported.</span></span>|
|<span data-ttu-id="409f3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="409f3-117">Application</span></span>|<span data-ttu-id="409f3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="409f3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="409f3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="409f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="409f3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="409f3-120">Request headers</span></span>
|<span data-ttu-id="409f3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="409f3-121">Header</span></span>|<span data-ttu-id="409f3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="409f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="409f3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="409f3-123">Authorization</span></span>|<span data-ttu-id="409f3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="409f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="409f3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="409f3-125">Accept</span></span>|<span data-ttu-id="409f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="409f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="409f3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="409f3-127">Request body</span></span>
<span data-ttu-id="409f3-128">В тексте запроса добавьте представление объекта объекта enrollmentprofile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="409f3-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="409f3-129">В следующей таблице приведены свойства, необходимые при создании объекта enrollmentprofile.</span><span class="sxs-lookup"><span data-stu-id="409f3-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="409f3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="409f3-130">Property</span></span>|<span data-ttu-id="409f3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="409f3-131">Type</span></span>|<span data-ttu-id="409f3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="409f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="409f3-133">id</span><span class="sxs-lookup"><span data-stu-id="409f3-133">id</span></span>|<span data-ttu-id="409f3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="409f3-134">String</span></span>|<span data-ttu-id="409f3-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="409f3-135">The GUID for the object</span></span>|
|<span data-ttu-id="409f3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="409f3-136">displayName</span></span>|<span data-ttu-id="409f3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="409f3-137">String</span></span>|<span data-ttu-id="409f3-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="409f3-138">Name of the profile</span></span>|
|<span data-ttu-id="409f3-139">description</span><span class="sxs-lookup"><span data-stu-id="409f3-139">description</span></span>|<span data-ttu-id="409f3-140">Строка</span><span class="sxs-lookup"><span data-stu-id="409f3-140">String</span></span>|<span data-ttu-id="409f3-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="409f3-141">Description of the profile</span></span>|
|<span data-ttu-id="409f3-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="409f3-142">requiresUserAuthentication</span></span>|<span data-ttu-id="409f3-143">Логический</span><span class="sxs-lookup"><span data-stu-id="409f3-143">Boolean</span></span>|<span data-ttu-id="409f3-144">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="409f3-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="409f3-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="409f3-145">configurationEndpointUrl</span></span>|<span data-ttu-id="409f3-146">Строка</span><span class="sxs-lookup"><span data-stu-id="409f3-146">String</span></span>|<span data-ttu-id="409f3-147">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="409f3-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="409f3-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="409f3-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="409f3-149">Логический</span><span class="sxs-lookup"><span data-stu-id="409f3-149">Boolean</span></span>|<span data-ttu-id="409f3-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="409f3-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="409f3-151">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="409f3-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="409f3-152">Логический</span><span class="sxs-lookup"><span data-stu-id="409f3-152">Boolean</span></span>|<span data-ttu-id="409f3-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="409f3-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="409f3-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="409f3-154">Response</span></span>
<span data-ttu-id="409f3-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="409f3-155">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="409f3-156">Пример</span><span class="sxs-lookup"><span data-stu-id="409f3-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="409f3-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="409f3-157">Request</span></span>
<span data-ttu-id="409f3-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="409f3-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="409f3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="409f3-159">Response</span></span>
<span data-ttu-id="409f3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="409f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





