---
title: Создание depEnrollmentProfile
description: Создайте новый объект depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72dd66b0cb453966f1c6701e1ae5b0316506f508
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149921"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="a0297-103">Создание depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a0297-103">Create depEnrollmentProfile</span></span>

<span data-ttu-id="a0297-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0297-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0297-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0297-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0297-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0297-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0297-107">Создайте новый [объект depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0297-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0297-108">Prerequisites</span></span>
<span data-ttu-id="a0297-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0297-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0297-111">Permission type</span></span>|<span data-ttu-id="a0297-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0297-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0297-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0297-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0297-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0297-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a0297-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0297-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0297-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0297-116">Not supported.</span></span>|
|<span data-ttu-id="a0297-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a0297-117">Application</span></span>|<span data-ttu-id="a0297-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0297-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0297-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0297-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a0297-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0297-120">Request headers</span></span>
|<span data-ttu-id="a0297-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0297-121">Header</span></span>|<span data-ttu-id="a0297-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a0297-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0297-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0297-123">Authorization</span></span>|<span data-ttu-id="a0297-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0297-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0297-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a0297-125">Accept</span></span>|<span data-ttu-id="a0297-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0297-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0297-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0297-127">Request body</span></span>
<span data-ttu-id="a0297-128">В теле запроса поставляем представление JSON для объекта depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a0297-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="a0297-129">В следующей таблице показаны свойства, необходимые при создании depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a0297-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="a0297-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0297-130">Property</span></span>|<span data-ttu-id="a0297-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a0297-131">Type</span></span>|<span data-ttu-id="a0297-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a0297-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0297-133">id</span><span class="sxs-lookup"><span data-stu-id="a0297-133">id</span></span>|<span data-ttu-id="a0297-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a0297-134">String</span></span>|<span data-ttu-id="a0297-135">GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a0297-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a0297-136">displayName</span></span>|<span data-ttu-id="a0297-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a0297-137">String</span></span>|<span data-ttu-id="a0297-138">Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a0297-139">description</span><span class="sxs-lookup"><span data-stu-id="a0297-139">description</span></span>|<span data-ttu-id="a0297-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a0297-140">String</span></span>|<span data-ttu-id="a0297-141">Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a0297-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="a0297-142">requiresUserAuthentication</span></span>|<span data-ttu-id="a0297-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-143">Boolean</span></span>|<span data-ttu-id="a0297-144">Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a0297-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="a0297-145">configurationEndpointUrl</span></span>|<span data-ttu-id="a0297-146">Строка</span><span class="sxs-lookup"><span data-stu-id="a0297-146">String</span></span>|<span data-ttu-id="a0297-147">URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a0297-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="a0297-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="a0297-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-149">Boolean</span></span>|<span data-ttu-id="a0297-150">Указывает на проверку подлинности с помощью помощника установки Apple вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="a0297-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="a0297-151">Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a0297-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="a0297-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="a0297-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-153">Boolean</span></span>|<span data-ttu-id="a0297-154">Указывает, что портал компании необходим для устройств, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a0297-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a0297-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="a0297-155">isDefault</span></span>|<span data-ttu-id="a0297-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-156">Boolean</span></span>|<span data-ttu-id="a0297-157">Указывает, является ли это профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="a0297-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="a0297-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="a0297-158">supervisedModeEnabled</span></span>|<span data-ttu-id="a0297-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-159">Boolean</span></span>|<span data-ttu-id="a0297-160">Режим Под контролем, True, чтобы включить, ложные в противном случае.</span><span class="sxs-lookup"><span data-stu-id="a0297-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="a0297-161">Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях.</span><span class="sxs-lookup"><span data-stu-id="a0297-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="a0297-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="a0297-162">supportDepartment</span></span>|<span data-ttu-id="a0297-163">Строка</span><span class="sxs-lookup"><span data-stu-id="a0297-163">String</span></span>|<span data-ttu-id="a0297-164">Сведения отдела поддержки</span><span class="sxs-lookup"><span data-stu-id="a0297-164">Support department information</span></span>|
|<span data-ttu-id="a0297-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-165">passCodeDisabled</span></span>|<span data-ttu-id="a0297-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-166">Boolean</span></span>|<span data-ttu-id="a0297-167">Указывает отключение области установки passcode</span><span class="sxs-lookup"><span data-stu-id="a0297-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="a0297-168">isMandatory</span></span>|<span data-ttu-id="a0297-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-169">Boolean</span></span>|<span data-ttu-id="a0297-170">Указывает, является ли профиль обязательным</span><span class="sxs-lookup"><span data-stu-id="a0297-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="a0297-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-171">locationDisabled</span></span>|<span data-ttu-id="a0297-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-172">Boolean</span></span>|<span data-ttu-id="a0297-173">Указывает, отключена ли панорама установки службы расположения</span><span class="sxs-lookup"><span data-stu-id="a0297-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a0297-174">supportPhoneNumber</span></span>|<span data-ttu-id="a0297-175">Строка</span><span class="sxs-lookup"><span data-stu-id="a0297-175">String</span></span>|<span data-ttu-id="a0297-176">Номер телефона поддержки</span><span class="sxs-lookup"><span data-stu-id="a0297-176">Support phone number</span></span>|
|<span data-ttu-id="a0297-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="a0297-177">iTunesPairingMode</span></span>|<span data-ttu-id="a0297-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="a0297-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="a0297-179">Указывает режим сопряжения iTunes.</span><span class="sxs-lookup"><span data-stu-id="a0297-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="a0297-180">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="a0297-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="a0297-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-181">profileRemovalDisabled</span></span>|<span data-ttu-id="a0297-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-182">Boolean</span></span>|<span data-ttu-id="a0297-183">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="a0297-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="a0297-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="a0297-184">managementCertificates</span></span>|<span data-ttu-id="a0297-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span><span class="sxs-lookup"><span data-stu-id="a0297-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="a0297-186">Сертификаты управления для Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="a0297-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="a0297-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a0297-187">restoreBlocked</span></span>|<span data-ttu-id="a0297-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-188">Boolean</span></span>|<span data-ttu-id="a0297-189">Указывает, заблокирована ли настройка области восстановления</span><span class="sxs-lookup"><span data-stu-id="a0297-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="a0297-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="a0297-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-191">Boolean</span></span>|<span data-ttu-id="a0297-192">Указывает, отключено ли восстановление с Android</span><span class="sxs-lookup"><span data-stu-id="a0297-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="a0297-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-193">appleIdDisabled</span></span>|<span data-ttu-id="a0297-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-194">Boolean</span></span>|<span data-ttu-id="a0297-195">Указывает, отключена ли области установки apple id</span><span class="sxs-lookup"><span data-stu-id="a0297-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="a0297-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-197">Boolean</span></span>|<span data-ttu-id="a0297-198">Указывает, отключено ли области установки "Условия и условия"</span><span class="sxs-lookup"><span data-stu-id="a0297-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-199">touchIdDisabled</span></span>|<span data-ttu-id="a0297-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-200">Boolean</span></span>|<span data-ttu-id="a0297-201">Указывает, отключена ли настройка сенсорного id</span><span class="sxs-lookup"><span data-stu-id="a0297-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-202">applePayDisabled</span></span>|<span data-ttu-id="a0297-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-203">Boolean</span></span>|<span data-ttu-id="a0297-204">Указывает, отключена ли система установки apple pay</span><span class="sxs-lookup"><span data-stu-id="a0297-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-205">zoomDisabled</span></span>|<span data-ttu-id="a0297-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-206">Boolean</span></span>|<span data-ttu-id="a0297-207">Указывает, отключена ли панорама настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="a0297-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-208">siriDisabled</span></span>|<span data-ttu-id="a0297-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-209">Boolean</span></span>|<span data-ttu-id="a0297-210">Указывает, отключено ли области настройки siri</span><span class="sxs-lookup"><span data-stu-id="a0297-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-211">diagnosticsDisabled</span></span>|<span data-ttu-id="a0297-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-212">Boolean</span></span>|<span data-ttu-id="a0297-213">Указывает отключение области настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="a0297-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="a0297-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="a0297-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-215">Boolean</span></span>|<span data-ttu-id="a0297-216">Указывает, отключена ли регистрация ОС Mac</span><span class="sxs-lookup"><span data-stu-id="a0297-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="a0297-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="a0297-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="a0297-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-218">Boolean</span></span>|<span data-ttu-id="a0297-219">Указывает, отключено ли хранилище файлов ОС Mac</span><span class="sxs-lookup"><span data-stu-id="a0297-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="a0297-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="a0297-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="a0297-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-221">Boolean</span></span>|<span data-ttu-id="a0297-222">Указывает, нужно ли устройству ждать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="a0297-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="a0297-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="a0297-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="a0297-224">Int32</span><span class="sxs-lookup"><span data-stu-id="a0297-224">Int32</span></span>|<span data-ttu-id="a0297-225">Это указывает максимальное число пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="a0297-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="a0297-226">Применяется только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="a0297-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="a0297-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="a0297-227">enableSharedIPad</span></span>|<span data-ttu-id="a0297-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0297-228">Boolean</span></span>|<span data-ttu-id="a0297-229">Это указывает, должно ли устройство быть зарегистрированным в режиме, который включает несколько сценариев пользователей.</span><span class="sxs-lookup"><span data-stu-id="a0297-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="a0297-230">Применимо только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="a0297-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="a0297-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0297-231">Response</span></span>
<span data-ttu-id="a0297-232">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a0297-232">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0297-233">Пример</span><span class="sxs-lookup"><span data-stu-id="a0297-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0297-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0297-234">Request</span></span>
<span data-ttu-id="a0297-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0297-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a><span data-ttu-id="a0297-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0297-236">Response</span></span>
<span data-ttu-id="a0297-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0297-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1403

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```




