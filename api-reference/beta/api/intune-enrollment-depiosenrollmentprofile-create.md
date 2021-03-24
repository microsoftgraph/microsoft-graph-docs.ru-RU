---
title: Создание depIOSEnrollmentProfile
description: Создание нового объекта depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a8f3e63b84132f5547c450b21a3cc8a44149369
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145987"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="52e8e-103">Создание depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="52e8e-103">Create depIOSEnrollmentProfile</span></span>

<span data-ttu-id="52e8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52e8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52e8e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52e8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52e8e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52e8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52e8e-107">Создание нового [объекта depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52e8e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52e8e-108">Prerequisites</span></span>
<span data-ttu-id="52e8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e8e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52e8e-111">Permission type</span></span>|<span data-ttu-id="52e8e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52e8e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52e8e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52e8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52e8e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e8e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="52e8e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52e8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52e8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52e8e-116">Not supported.</span></span>|
|<span data-ttu-id="52e8e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="52e8e-117">Application</span></span>|<span data-ttu-id="52e8e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e8e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52e8e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52e8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="52e8e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52e8e-120">Request headers</span></span>
|<span data-ttu-id="52e8e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52e8e-121">Header</span></span>|<span data-ttu-id="52e8e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52e8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52e8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52e8e-123">Authorization</span></span>|<span data-ttu-id="52e8e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52e8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52e8e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52e8e-125">Accept</span></span>|<span data-ttu-id="52e8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52e8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52e8e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52e8e-127">Request body</span></span>
<span data-ttu-id="52e8e-128">В теле запроса поставляем представление JSON для объекта depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="52e8e-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="52e8e-129">В следующей таблице показаны свойства, необходимые при создании depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="52e8e-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="52e8e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52e8e-130">Property</span></span>|<span data-ttu-id="52e8e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52e8e-131">Type</span></span>|<span data-ttu-id="52e8e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52e8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e8e-133">id</span><span class="sxs-lookup"><span data-stu-id="52e8e-133">id</span></span>|<span data-ttu-id="52e8e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-134">String</span></span>|<span data-ttu-id="52e8e-135">GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e8e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="52e8e-136">displayName</span></span>|<span data-ttu-id="52e8e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-137">String</span></span>|<span data-ttu-id="52e8e-138">Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e8e-139">description</span><span class="sxs-lookup"><span data-stu-id="52e8e-139">description</span></span>|<span data-ttu-id="52e8e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-140">String</span></span>|<span data-ttu-id="52e8e-141">Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e8e-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="52e8e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="52e8e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-143">Boolean</span></span>|<span data-ttu-id="52e8e-144">Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e8e-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="52e8e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="52e8e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-146">String</span></span>|<span data-ttu-id="52e8e-147">URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e8e-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="52e8e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="52e8e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-149">Boolean</span></span>|<span data-ttu-id="52e8e-150">Указывает на проверку подлинности с помощью помощника установки Apple вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="52e8e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="52e8e-151">Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e8e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="52e8e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="52e8e-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-153">Boolean</span></span>|<span data-ttu-id="52e8e-154">Указывает, что портал компании необходим для устройств, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="52e8e-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="52e8e-155">isDefault</span></span>|<span data-ttu-id="52e8e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-156">Boolean</span></span>|<span data-ttu-id="52e8e-157">Указывает, является ли это профилем по умолчанию, унаследованной от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-158">supervisedModeEnabled</span></span>|<span data-ttu-id="52e8e-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-159">Boolean</span></span>|<span data-ttu-id="52e8e-160">Режим Под контролем, True, чтобы включить, ложные в противном случае.</span><span class="sxs-lookup"><span data-stu-id="52e8e-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="52e8e-161">Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях.</span><span class="sxs-lookup"><span data-stu-id="52e8e-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="52e8e-162">Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="52e8e-163">supportDepartment</span></span>|<span data-ttu-id="52e8e-164">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-164">String</span></span>|<span data-ttu-id="52e8e-165">Сведения отдела поддержки, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="52e8e-166">isMandatory</span></span>|<span data-ttu-id="52e8e-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-167">Boolean</span></span>|<span data-ttu-id="52e8e-168">Указывает, является ли профиль обязательным, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-169">locationDisabled</span></span>|<span data-ttu-id="52e8e-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-170">Boolean</span></span>|<span data-ttu-id="52e8e-171">Указывает, отключено ли области установки службы расположения из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="52e8e-172">supportPhoneNumber</span></span>|<span data-ttu-id="52e8e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-173">String</span></span>|<span data-ttu-id="52e8e-174">Номер телефона поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-175">profileRemovalDisabled</span></span>|<span data-ttu-id="52e8e-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-176">Boolean</span></span>|<span data-ttu-id="52e8e-177">Указывает, отключен ли параметр удаления профиля, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="52e8e-178">restoreBlocked</span></span>|<span data-ttu-id="52e8e-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-179">Boolean</span></span>|<span data-ttu-id="52e8e-180">Указывает, заблокирована ли настройка области восстановления, наследуемая [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-181">appleIdDisabled</span></span>|<span data-ttu-id="52e8e-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-182">Boolean</span></span>|<span data-ttu-id="52e8e-183">Указывает, отключена ли система установки apple id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="52e8e-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-185">Boolean</span></span>|<span data-ttu-id="52e8e-186">Указывает, отключено ли области установки "Условия и условия", унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-187">touchIdDisabled</span></span>|<span data-ttu-id="52e8e-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-188">Boolean</span></span>|<span data-ttu-id="52e8e-189">Указывает, отключена ли для настройки сенсорного id наследуемая из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-190">applePayDisabled</span></span>|<span data-ttu-id="52e8e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-191">Boolean</span></span>|<span data-ttu-id="52e8e-192">Указывает, отключена ли система установки apple pay inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-193">siriDisabled</span></span>|<span data-ttu-id="52e8e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-194">Boolean</span></span>|<span data-ttu-id="52e8e-195">Указывает, отключена ли настройка siri из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-196">diagnosticsDisabled</span></span>|<span data-ttu-id="52e8e-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-197">Boolean</span></span>|<span data-ttu-id="52e8e-198">Указывает, отключено ли области настройки диагностики, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="52e8e-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-200">Boolean</span></span>|<span data-ttu-id="52e8e-201">Указывает, отключен ли экран настройки displaytone, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-202">privacyPaneDisabled</span></span>|<span data-ttu-id="52e8e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-203">Boolean</span></span>|<span data-ttu-id="52e8e-204">Указывает, отключен ли экран конфиденциальности, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="52e8e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-206">Boolean</span></span>|<span data-ttu-id="52e8e-207">Указывает, отключена ли установка расстановки времени на экране, наследуемая [из depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="52e8e-208">deviceNameTemplate</span></span>|<span data-ttu-id="52e8e-209">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-209">String</span></span>|<span data-ttu-id="52e8e-210">Задает буквальный или имя шаблон.</span><span class="sxs-lookup"><span data-stu-id="52e8e-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="52e8e-211">Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="52e8e-212">configurationWebUrl</span></span>|<span data-ttu-id="52e8e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-213">Boolean</span></span>|<span data-ttu-id="52e8e-214">URL-адрес для входа помощника установки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="52e8e-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="52e8e-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="52e8e-215">iTunesPairingMode</span></span>|<span data-ttu-id="52e8e-216">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="52e8e-216">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="52e8e-217">Указывает режим сопряжения iTunes.</span><span class="sxs-lookup"><span data-stu-id="52e8e-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="52e8e-218">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="52e8e-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="52e8e-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="52e8e-219">managementCertificates</span></span>|<span data-ttu-id="52e8e-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span><span class="sxs-lookup"><span data-stu-id="52e8e-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="52e8e-221">Сертификаты управления для Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="52e8e-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="52e8e-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="52e8e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-223">Boolean</span></span>|<span data-ttu-id="52e8e-224">Указывает, отключено ли восстановление с Android</span><span class="sxs-lookup"><span data-stu-id="52e8e-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="52e8e-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="52e8e-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="52e8e-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-226">Boolean</span></span>|<span data-ttu-id="52e8e-227">Указывает, нужно ли устройству ждать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="52e8e-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="52e8e-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="52e8e-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="52e8e-229">Int32</span><span class="sxs-lookup"><span data-stu-id="52e8e-229">Int32</span></span>|<span data-ttu-id="52e8e-230">Это указывает максимальное число пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="52e8e-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="52e8e-231">Применяется только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="52e8e-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="52e8e-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="52e8e-232">enableSharedIPad</span></span>|<span data-ttu-id="52e8e-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-233">Boolean</span></span>|<span data-ttu-id="52e8e-234">Это указывает, должно ли устройство быть зарегистрированным в режиме, который включает несколько сценариев пользователей.</span><span class="sxs-lookup"><span data-stu-id="52e8e-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="52e8e-235">Применимо только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="52e8e-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="52e8e-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="52e8e-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="52e8e-237">Строка</span><span class="sxs-lookup"><span data-stu-id="52e8e-237">String</span></span>|<span data-ttu-id="52e8e-238">Если установлено, указывается, какой маркер Vpp следует использовать для развертывания лицензирования портала компании w/device.</span><span class="sxs-lookup"><span data-stu-id="52e8e-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="52e8e-239">Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="52e8e-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="52e8e-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="52e8e-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="52e8e-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-241">Boolean</span></span>|<span data-ttu-id="52e8e-242">Сообщает устройству включить режим одного приложения и применить блокировку приложения во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="52e8e-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="52e8e-243">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="52e8e-243">Default is false.</span></span> <span data-ttu-id="52e8e-244">Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal" и "companyPortalVppTokenId".</span><span class="sxs-lookup"><span data-stu-id="52e8e-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="52e8e-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="52e8e-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-246">Boolean</span></span>|<span data-ttu-id="52e8e-247">Указывает, отключен ли экран чувствительности домашней кнопки</span><span class="sxs-lookup"><span data-stu-id="52e8e-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="52e8e-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="52e8e-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-249">Boolean</span></span>|<span data-ttu-id="52e8e-250">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="52e8e-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="52e8e-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="52e8e-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-252">Boolean</span></span>|<span data-ttu-id="52e8e-253">Указывает, отключен ли экран установки бортовой установки</span><span class="sxs-lookup"><span data-stu-id="52e8e-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="52e8e-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="52e8e-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-255">Boolean</span></span>|<span data-ttu-id="52e8e-256">Указывает, отключен ли экран SIMSetup</span><span class="sxs-lookup"><span data-stu-id="52e8e-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="52e8e-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="52e8e-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-258">Boolean</span></span>|<span data-ttu-id="52e8e-259">Указывает, отключен ли экран обязательного обновления sofware</span><span class="sxs-lookup"><span data-stu-id="52e8e-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="52e8e-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="52e8e-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-261">Boolean</span></span>|<span data-ttu-id="52e8e-262">Указывает, отключен ли экран переноса часов</span><span class="sxs-lookup"><span data-stu-id="52e8e-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="52e8e-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="52e8e-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-264">Boolean</span></span>|<span data-ttu-id="52e8e-265">Указывает, отключен ли экран Apperance</span><span class="sxs-lookup"><span data-stu-id="52e8e-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="52e8e-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="52e8e-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-267">Boolean</span></span>|<span data-ttu-id="52e8e-268">Указывает, отключен ли экран express Language</span><span class="sxs-lookup"><span data-stu-id="52e8e-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="52e8e-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="52e8e-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-270">Boolean</span></span>|<span data-ttu-id="52e8e-271">Указывает, отключен ли предпочтительный языковой экран</span><span class="sxs-lookup"><span data-stu-id="52e8e-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="52e8e-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="52e8e-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-273">Boolean</span></span>|<span data-ttu-id="52e8e-274">Указывает, отключена ли миграция устройства на устройство</span><span class="sxs-lookup"><span data-stu-id="52e8e-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="52e8e-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="52e8e-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-276">Boolean</span></span>|<span data-ttu-id="52e8e-277">Указывает, отключен ли экран Weclome</span><span class="sxs-lookup"><span data-stu-id="52e8e-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="52e8e-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-278">passCodeDisabled</span></span>|<span data-ttu-id="52e8e-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-279">Boolean</span></span>|<span data-ttu-id="52e8e-280">Указывает отключение области установки passcode</span><span class="sxs-lookup"><span data-stu-id="52e8e-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="52e8e-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-281">zoomDisabled</span></span>|<span data-ttu-id="52e8e-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-282">Boolean</span></span>|<span data-ttu-id="52e8e-283">Указывает, отключена ли панорама настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="52e8e-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="52e8e-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="52e8e-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-285">Boolean</span></span>|<span data-ttu-id="52e8e-286">Указывает, отключен ли экран Weclome</span><span class="sxs-lookup"><span data-stu-id="52e8e-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="52e8e-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="52e8e-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="52e8e-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e8e-288">Boolean</span></span>|<span data-ttu-id="52e8e-289">Указывает, отключен ли экран Weclome</span><span class="sxs-lookup"><span data-stu-id="52e8e-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="52e8e-290">Отклик</span><span class="sxs-lookup"><span data-stu-id="52e8e-290">Response</span></span>
<span data-ttu-id="52e8e-291">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="52e8e-291">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52e8e-292">Пример</span><span class="sxs-lookup"><span data-stu-id="52e8e-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="52e8e-293">Запрос</span><span class="sxs-lookup"><span data-stu-id="52e8e-293">Request</span></span>
<span data-ttu-id="52e8e-294">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52e8e-294">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 2108

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="52e8e-295">Отклик</span><span class="sxs-lookup"><span data-stu-id="52e8e-295">Response</span></span>
<span data-ttu-id="52e8e-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52e8e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2157

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```




