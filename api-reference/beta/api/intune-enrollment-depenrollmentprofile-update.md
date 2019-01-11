---
title: Обновление depEnrollmentProfile
description: Обновление свойства объекта depEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2d444f6c94eb8dd047e000004f5dbf58dc3c302d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866187"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="43e31-103">Обновление depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="43e31-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="43e31-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="43e31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43e31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43e31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43e31-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="43e31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43e31-107">Обновление свойства объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="43e31-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43e31-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43e31-108">Prerequisites</span></span>
<span data-ttu-id="43e31-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43e31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43e31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43e31-111">Permission type</span></span>|<span data-ttu-id="43e31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43e31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43e31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43e31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43e31-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e31-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43e31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43e31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43e31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43e31-116">Not supported.</span></span>|
|<span data-ttu-id="43e31-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43e31-117">Application</span></span>|<span data-ttu-id="43e31-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43e31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43e31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43e31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="43e31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43e31-120">Request headers</span></span>
|<span data-ttu-id="43e31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43e31-121">Header</span></span>|<span data-ttu-id="43e31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43e31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43e31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43e31-123">Authorization</span></span>|<span data-ttu-id="43e31-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="43e31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43e31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43e31-125">Accept</span></span>|<span data-ttu-id="43e31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43e31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43e31-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43e31-127">Request body</span></span>
<span data-ttu-id="43e31-128">В тексте запроса укажите представление JSON для объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="43e31-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="43e31-129">В следующей таблице показаны свойства, которые необходимы для создания [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="43e31-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="43e31-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="43e31-130">Property</span></span>|<span data-ttu-id="43e31-131">Тип</span><span class="sxs-lookup"><span data-stu-id="43e31-131">Type</span></span>|<span data-ttu-id="43e31-132">Описание</span><span class="sxs-lookup"><span data-stu-id="43e31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43e31-133">id</span><span class="sxs-lookup"><span data-stu-id="43e31-133">id</span></span>|<span data-ttu-id="43e31-134">Строка</span><span class="sxs-lookup"><span data-stu-id="43e31-134">String</span></span>|<span data-ttu-id="43e31-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43e31-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43e31-136">displayName</span><span class="sxs-lookup"><span data-stu-id="43e31-136">displayName</span></span>|<span data-ttu-id="43e31-137">Строка</span><span class="sxs-lookup"><span data-stu-id="43e31-137">String</span></span>|<span data-ttu-id="43e31-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43e31-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43e31-139">описание</span><span class="sxs-lookup"><span data-stu-id="43e31-139">description</span></span>|<span data-ttu-id="43e31-140">Строка</span><span class="sxs-lookup"><span data-stu-id="43e31-140">String</span></span>|<span data-ttu-id="43e31-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43e31-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43e31-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="43e31-142">requiresUserAuthentication</span></span>|<span data-ttu-id="43e31-143">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-143">Boolean</span></span>|<span data-ttu-id="43e31-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43e31-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43e31-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="43e31-145">configurationEndpointUrl</span></span>|<span data-ttu-id="43e31-146">Строка</span><span class="sxs-lookup"><span data-stu-id="43e31-146">String</span></span>|<span data-ttu-id="43e31-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43e31-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43e31-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="43e31-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="43e31-149">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-149">Boolean</span></span>|<span data-ttu-id="43e31-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="43e31-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="43e31-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43e31-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43e31-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="43e31-152">isDefault</span></span>|<span data-ttu-id="43e31-153">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-153">Boolean</span></span>|<span data-ttu-id="43e31-154">Указывает, является ли профиля по умолчанию</span><span class="sxs-lookup"><span data-stu-id="43e31-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="43e31-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="43e31-155">supervisedModeEnabled</span></span>|<span data-ttu-id="43e31-156">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-156">Boolean</span></span>|<span data-ttu-id="43e31-157">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="43e31-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="43e31-158">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="43e31-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="43e31-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="43e31-159">supportDepartment</span></span>|<span data-ttu-id="43e31-160">Строка</span><span class="sxs-lookup"><span data-stu-id="43e31-160">String</span></span>|<span data-ttu-id="43e31-161">Сведения о поддержке отдела</span><span class="sxs-lookup"><span data-stu-id="43e31-161">Support department information</span></span>|
|<span data-ttu-id="43e31-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-162">passCodeDisabled</span></span>|<span data-ttu-id="43e31-163">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-163">Boolean</span></span>|<span data-ttu-id="43e31-164">Указывает, если область настройки секретный код отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="43e31-165">isMandatory</span></span>|<span data-ttu-id="43e31-166">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-166">Boolean</span></span>|<span data-ttu-id="43e31-167">Указывает, является ли обязательных профилей</span><span class="sxs-lookup"><span data-stu-id="43e31-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="43e31-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-168">locationDisabled</span></span>|<span data-ttu-id="43e31-169">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-169">Boolean</span></span>|<span data-ttu-id="43e31-170">Указывает, если область настройки расположения службы отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="43e31-171">supportPhoneNumber</span></span>|<span data-ttu-id="43e31-172">Строка</span><span class="sxs-lookup"><span data-stu-id="43e31-172">String</span></span>|<span data-ttu-id="43e31-173">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="43e31-173">Support phone number</span></span>|
|<span data-ttu-id="43e31-174">iTunesPairingMode.</span><span class="sxs-lookup"><span data-stu-id="43e31-174">iTunesPairingMode</span></span>|<span data-ttu-id="43e31-175">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="43e31-175">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="43e31-176">Указывает iTunes, режим связывания.</span><span class="sxs-lookup"><span data-stu-id="43e31-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="43e31-177">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="43e31-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="43e31-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-178">profileRemovalDisabled</span></span>|<span data-ttu-id="43e31-179">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-179">Boolean</span></span>|<span data-ttu-id="43e31-180">Указывает, если параметр удаления профиль отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="43e31-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="43e31-181">managementCertificates</span></span>|<span data-ttu-id="43e31-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="43e31-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="43e31-183">Управление сертификатами для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="43e31-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="43e31-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="43e31-184">restoreBlocked</span></span>|<span data-ttu-id="43e31-185">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-185">Boolean</span></span>|<span data-ttu-id="43e31-186">Указывает, если область настройки восстановления блокируется</span><span class="sxs-lookup"><span data-stu-id="43e31-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="43e31-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="43e31-188">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-188">Boolean</span></span>|<span data-ttu-id="43e31-189">Указывает, если отключено восстановление из Android (en)</span><span class="sxs-lookup"><span data-stu-id="43e31-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="43e31-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-190">appleIdDisabled</span></span>|<span data-ttu-id="43e31-191">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-191">Boolean</span></span>|<span data-ttu-id="43e31-192">Указывает, если область настройки идентификатор Apple отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="43e31-194">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-194">Boolean</span></span>|<span data-ttu-id="43e31-195">Указывает, если отключено «Сроками и условиями» область настройки</span><span class="sxs-lookup"><span data-stu-id="43e31-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-196">touchIdDisabled</span></span>|<span data-ttu-id="43e31-197">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-197">Boolean</span></span>|<span data-ttu-id="43e31-198">Указывает, если область настройки идентификатор сенсорного ввода отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-199">applePayDisabled</span></span>|<span data-ttu-id="43e31-200">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-200">Boolean</span></span>|<span data-ttu-id="43e31-201">Указывает, если область настройки оплаты Apple отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-202">zoomDisabled</span></span>|<span data-ttu-id="43e31-203">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-203">Boolean</span></span>|<span data-ttu-id="43e31-204">Указывает, если область настройки масштаба отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-205">siriDisabled</span></span>|<span data-ttu-id="43e31-206">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-206">Boolean</span></span>|<span data-ttu-id="43e31-207">Указывает, если область настроек siri отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-208">diagnosticsDisabled</span></span>|<span data-ttu-id="43e31-209">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-209">Boolean</span></span>|<span data-ttu-id="43e31-210">Указывает, если область настройки диагностики отключен</span><span class="sxs-lookup"><span data-stu-id="43e31-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="43e31-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="43e31-212">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-212">Boolean</span></span>|<span data-ttu-id="43e31-213">Указывает, отключена при регистрации Mac OS</span><span class="sxs-lookup"><span data-stu-id="43e31-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="43e31-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="43e31-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="43e31-215">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-215">Boolean</span></span>|<span data-ttu-id="43e31-216">Указывает, если отключено хранилище файлов Mac OS</span><span class="sxs-lookup"><span data-stu-id="43e31-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="43e31-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="43e31-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="43e31-218">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-218">Boolean</span></span>|<span data-ttu-id="43e31-219">Указывает, если устройство необходимо подождать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="43e31-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="43e31-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="43e31-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="43e31-221">Int32</span><span class="sxs-lookup"><span data-stu-id="43e31-221">Int32</span></span>|<span data-ttu-id="43e31-222">Это указывает максимальное количество пользователей, которые могут использовать общие iPad.</span><span class="sxs-lookup"><span data-stu-id="43e31-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="43e31-223">Применим только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="43e31-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="43e31-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="43e31-224">enableSharedIPad</span></span>|<span data-ttu-id="43e31-225">Логический</span><span class="sxs-lookup"><span data-stu-id="43e31-225">Boolean</span></span>|<span data-ttu-id="43e31-226">Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии.</span><span class="sxs-lookup"><span data-stu-id="43e31-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="43e31-227">Применим только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="43e31-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="43e31-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="43e31-228">Response</span></span>
<span data-ttu-id="43e31-229">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="43e31-229">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43e31-230">Пример</span><span class="sxs-lookup"><span data-stu-id="43e31-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="43e31-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="43e31-231">Request</span></span>
<span data-ttu-id="43e31-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43e31-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43e31-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="43e31-233">Response</span></span>
<span data-ttu-id="43e31-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="43e31-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





