---
title: Обновление enrollmentProfile
description: Обновление свойства объекта enrollmentProfile.
ms.openlocfilehash: 6d8d0b6650c1094f1d2c46ab197eeb1781e097d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080653"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="16eae-103">Обновление enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="16eae-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="16eae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16eae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16eae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16eae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16eae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16eae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16eae-107">Обновление свойства объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16eae-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16eae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16eae-108">Prerequisites</span></span>
<span data-ttu-id="16eae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16eae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16eae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16eae-111">Permission type</span></span>|<span data-ttu-id="16eae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16eae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16eae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16eae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16eae-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16eae-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16eae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16eae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16eae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16eae-116">Not supported.</span></span>|
|<span data-ttu-id="16eae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16eae-117">Application</span></span>|<span data-ttu-id="16eae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16eae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16eae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16eae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="16eae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16eae-120">Request headers</span></span>
|<span data-ttu-id="16eae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16eae-121">Header</span></span>|<span data-ttu-id="16eae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16eae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16eae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16eae-123">Authorization</span></span>|<span data-ttu-id="16eae-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="16eae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16eae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16eae-125">Accept</span></span>|<span data-ttu-id="16eae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16eae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16eae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16eae-127">Request body</span></span>
<span data-ttu-id="16eae-128">В тексте запроса укажите представление JSON для объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="16eae-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="16eae-129">В следующей таблице показаны свойства, которые необходимы для создания [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="16eae-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="16eae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16eae-130">Property</span></span>|<span data-ttu-id="16eae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16eae-131">Type</span></span>|<span data-ttu-id="16eae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16eae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16eae-133">id</span><span class="sxs-lookup"><span data-stu-id="16eae-133">id</span></span>|<span data-ttu-id="16eae-134">Строка</span><span class="sxs-lookup"><span data-stu-id="16eae-134">String</span></span>|<span data-ttu-id="16eae-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="16eae-135">The GUID for the object</span></span>|
|<span data-ttu-id="16eae-136">displayName</span><span class="sxs-lookup"><span data-stu-id="16eae-136">displayName</span></span>|<span data-ttu-id="16eae-137">String</span><span class="sxs-lookup"><span data-stu-id="16eae-137">String</span></span>|<span data-ttu-id="16eae-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="16eae-138">Name of the profile</span></span>|
|<span data-ttu-id="16eae-139">описание</span><span class="sxs-lookup"><span data-stu-id="16eae-139">description</span></span>|<span data-ttu-id="16eae-140">String</span><span class="sxs-lookup"><span data-stu-id="16eae-140">String</span></span>|<span data-ttu-id="16eae-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="16eae-141">Description of the profile</span></span>|
|<span data-ttu-id="16eae-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="16eae-142">requiresUserAuthentication</span></span>|<span data-ttu-id="16eae-143">Логический</span><span class="sxs-lookup"><span data-stu-id="16eae-143">Boolean</span></span>|<span data-ttu-id="16eae-144">Указывает необходимость проверки подлинности пользователей в профиле</span><span class="sxs-lookup"><span data-stu-id="16eae-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="16eae-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="16eae-145">configurationEndpointUrl</span></span>|<span data-ttu-id="16eae-146">String</span><span class="sxs-lookup"><span data-stu-id="16eae-146">String</span></span>|<span data-ttu-id="16eae-147">URL-адрес конечной точки конфигурации для подачи заявок</span><span class="sxs-lookup"><span data-stu-id="16eae-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="16eae-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="16eae-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="16eae-149">Логический</span><span class="sxs-lookup"><span data-stu-id="16eae-149">Boolean</span></span>|<span data-ttu-id="16eae-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="16eae-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="16eae-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="16eae-151">Response</span></span>
<span data-ttu-id="16eae-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16eae-152">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16eae-153">Пример</span><span class="sxs-lookup"><span data-stu-id="16eae-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="16eae-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="16eae-154">Request</span></span>
<span data-ttu-id="16eae-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16eae-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 250

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="16eae-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="16eae-156">Response</span></span>
<span data-ttu-id="16eae-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="16eae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```





