---
title: Обновление depEnrollmentProfile
description: Обновление свойства объекта depEnrollmentProfile.
author: tfitzmac
ms.openlocfilehash: 06d6fc12379a7f26ed8baf0e24bf23ef696c067a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322514"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="251ba-103">Обновление depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="251ba-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="251ba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="251ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="251ba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="251ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="251ba-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="251ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="251ba-107">Обновление свойства объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="251ba-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="251ba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="251ba-108">Prerequisites</span></span>
<span data-ttu-id="251ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="251ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="251ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="251ba-111">Permission type</span></span>|<span data-ttu-id="251ba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="251ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="251ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="251ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="251ba-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="251ba-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="251ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="251ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="251ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="251ba-116">Not supported.</span></span>|
|<span data-ttu-id="251ba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="251ba-117">Application</span></span>|<span data-ttu-id="251ba-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="251ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="251ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="251ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="251ba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="251ba-120">Request headers</span></span>
|<span data-ttu-id="251ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="251ba-121">Header</span></span>|<span data-ttu-id="251ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="251ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="251ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="251ba-123">Authorization</span></span>|<span data-ttu-id="251ba-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="251ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="251ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="251ba-125">Accept</span></span>|<span data-ttu-id="251ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="251ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="251ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="251ba-127">Request body</span></span>
<span data-ttu-id="251ba-128">В тексте запроса укажите представление JSON для объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="251ba-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="251ba-129">В следующей таблице показаны свойства, которые необходимы для создания [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="251ba-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="251ba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="251ba-130">Property</span></span>|<span data-ttu-id="251ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="251ba-131">Type</span></span>|<span data-ttu-id="251ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="251ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="251ba-133">id</span><span class="sxs-lookup"><span data-stu-id="251ba-133">id</span></span>|<span data-ttu-id="251ba-134">Строка</span><span class="sxs-lookup"><span data-stu-id="251ba-134">String</span></span>|<span data-ttu-id="251ba-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="251ba-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="251ba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="251ba-136">displayName</span></span>|<span data-ttu-id="251ba-137">Строка</span><span class="sxs-lookup"><span data-stu-id="251ba-137">String</span></span>|<span data-ttu-id="251ba-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="251ba-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="251ba-139">описание</span><span class="sxs-lookup"><span data-stu-id="251ba-139">description</span></span>|<span data-ttu-id="251ba-140">Строка</span><span class="sxs-lookup"><span data-stu-id="251ba-140">String</span></span>|<span data-ttu-id="251ba-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="251ba-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="251ba-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="251ba-142">requiresUserAuthentication</span></span>|<span data-ttu-id="251ba-143">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-143">Boolean</span></span>|<span data-ttu-id="251ba-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="251ba-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="251ba-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="251ba-145">configurationEndpointUrl</span></span>|<span data-ttu-id="251ba-146">String.</span><span class="sxs-lookup"><span data-stu-id="251ba-146">String</span></span>|<span data-ttu-id="251ba-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="251ba-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="251ba-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="251ba-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="251ba-149">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-149">Boolean</span></span>|<span data-ttu-id="251ba-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="251ba-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="251ba-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="251ba-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="251ba-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="251ba-152">isDefault</span></span>|<span data-ttu-id="251ba-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="251ba-153">Boolean</span></span>|<span data-ttu-id="251ba-154">Указывает, является ли профиля по умолчанию</span><span class="sxs-lookup"><span data-stu-id="251ba-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="251ba-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="251ba-155">supervisedModeEnabled</span></span>|<span data-ttu-id="251ba-156">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-156">Boolean</span></span>|<span data-ttu-id="251ba-157">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="251ba-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="251ba-158">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="251ba-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="251ba-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="251ba-159">supportDepartment</span></span>|<span data-ttu-id="251ba-160">String.</span><span class="sxs-lookup"><span data-stu-id="251ba-160">String</span></span>|<span data-ttu-id="251ba-161">Сведения о поддержке отдела</span><span class="sxs-lookup"><span data-stu-id="251ba-161">Support department information</span></span>|
|<span data-ttu-id="251ba-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-162">passCodeDisabled</span></span>|<span data-ttu-id="251ba-163">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-163">Boolean</span></span>|<span data-ttu-id="251ba-164">Указывает, если область настройки секретный код отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="251ba-165">isMandatory</span></span>|<span data-ttu-id="251ba-166">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-166">Boolean</span></span>|<span data-ttu-id="251ba-167">Указывает, является ли обязательных профилей</span><span class="sxs-lookup"><span data-stu-id="251ba-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="251ba-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-168">locationDisabled</span></span>|<span data-ttu-id="251ba-169">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-169">Boolean</span></span>|<span data-ttu-id="251ba-170">Указывает, если область настройки расположения службы отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="251ba-171">supportPhoneNumber</span></span>|<span data-ttu-id="251ba-172">String.</span><span class="sxs-lookup"><span data-stu-id="251ba-172">String</span></span>|<span data-ttu-id="251ba-173">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="251ba-173">Support phone number</span></span>|
|<span data-ttu-id="251ba-174">iTunesPairingMode.</span><span class="sxs-lookup"><span data-stu-id="251ba-174">iTunesPairingMode</span></span>|<span data-ttu-id="251ba-175">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="251ba-175">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="251ba-176">Указывает iTunes, режим связывания.</span><span class="sxs-lookup"><span data-stu-id="251ba-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="251ba-177">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="251ba-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="251ba-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-178">profileRemovalDisabled</span></span>|<span data-ttu-id="251ba-179">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-179">Boolean</span></span>|<span data-ttu-id="251ba-180">Указывает, если параметр удаления профиль отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="251ba-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="251ba-181">managementCertificates</span></span>|<span data-ttu-id="251ba-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="251ba-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="251ba-183">Управление сертификатами для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="251ba-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="251ba-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="251ba-184">restoreBlocked</span></span>|<span data-ttu-id="251ba-185">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-185">Boolean</span></span>|<span data-ttu-id="251ba-186">Указывает, если область настройки восстановления блокируется</span><span class="sxs-lookup"><span data-stu-id="251ba-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="251ba-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="251ba-188">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-188">Boolean</span></span>|<span data-ttu-id="251ba-189">Указывает, если отключено восстановление из Android (en)</span><span class="sxs-lookup"><span data-stu-id="251ba-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="251ba-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-190">appleIdDisabled</span></span>|<span data-ttu-id="251ba-191">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-191">Boolean</span></span>|<span data-ttu-id="251ba-192">Указывает, если область настройки идентификатор Apple отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="251ba-194">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-194">Boolean</span></span>|<span data-ttu-id="251ba-195">Указывает, если отключено «Сроками и условиями» область настройки</span><span class="sxs-lookup"><span data-stu-id="251ba-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-196">touchIdDisabled</span></span>|<span data-ttu-id="251ba-197">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-197">Boolean</span></span>|<span data-ttu-id="251ba-198">Указывает, если область настройки идентификатор сенсорного ввода отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-199">applePayDisabled</span></span>|<span data-ttu-id="251ba-200">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-200">Boolean</span></span>|<span data-ttu-id="251ba-201">Указывает, если область настройки оплаты Apple отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-202">zoomDisabled</span></span>|<span data-ttu-id="251ba-203">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-203">Boolean</span></span>|<span data-ttu-id="251ba-204">Указывает, если область настройки масштаба отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-205">siriDisabled</span></span>|<span data-ttu-id="251ba-206">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-206">Boolean</span></span>|<span data-ttu-id="251ba-207">Указывает, если область настроек siri отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-208">diagnosticsDisabled</span></span>|<span data-ttu-id="251ba-209">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-209">Boolean</span></span>|<span data-ttu-id="251ba-210">Указывает, если область настройки диагностики отключен</span><span class="sxs-lookup"><span data-stu-id="251ba-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="251ba-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="251ba-212">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-212">Boolean</span></span>|<span data-ttu-id="251ba-213">Указывает, отключена при регистрации Mac OS</span><span class="sxs-lookup"><span data-stu-id="251ba-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="251ba-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="251ba-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="251ba-215">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-215">Boolean</span></span>|<span data-ttu-id="251ba-216">Указывает, если отключено хранилище файлов Mac OS</span><span class="sxs-lookup"><span data-stu-id="251ba-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="251ba-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="251ba-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="251ba-218">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-218">Boolean</span></span>|<span data-ttu-id="251ba-219">Указывает, если устройство необходимо подождать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="251ba-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="251ba-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="251ba-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="251ba-221">Int32</span><span class="sxs-lookup"><span data-stu-id="251ba-221">Int32</span></span>|<span data-ttu-id="251ba-222">Это указывает максимальное количество пользователей, которые могут использовать общие iPad.</span><span class="sxs-lookup"><span data-stu-id="251ba-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="251ba-223">Применим только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="251ba-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="251ba-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="251ba-224">enableSharedIPad</span></span>|<span data-ttu-id="251ba-225">Boolean.</span><span class="sxs-lookup"><span data-stu-id="251ba-225">Boolean</span></span>|<span data-ttu-id="251ba-226">Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии.</span><span class="sxs-lookup"><span data-stu-id="251ba-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="251ba-227">Применим только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="251ba-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="251ba-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="251ba-228">Response</span></span>
<span data-ttu-id="251ba-229">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="251ba-229">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="251ba-230">Пример</span><span class="sxs-lookup"><span data-stu-id="251ba-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="251ba-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="251ba-231">Request</span></span>
<span data-ttu-id="251ba-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="251ba-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1231

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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

### <a name="response"></a><span data-ttu-id="251ba-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="251ba-233">Response</span></span>
<span data-ttu-id="251ba-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="251ba-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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





