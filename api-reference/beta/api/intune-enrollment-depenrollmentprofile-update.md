---
title: Обновление depEnrollmentProfile
description: Обновление свойства объекта depEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f8bb392eba1ca79815d72baf9f89e790cb16d95
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419529"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="15b9a-103">Обновление depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15b9a-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="15b9a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15b9a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15b9a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b9a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15b9a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15b9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15b9a-107">Обновление свойства объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="15b9a-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15b9a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="15b9a-108">Prerequisites</span></span>
<span data-ttu-id="15b9a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15b9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15b9a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15b9a-111">Permission type</span></span>|<span data-ttu-id="15b9a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15b9a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15b9a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15b9a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15b9a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15b9a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15b9a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15b9a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15b9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b9a-116">Not supported.</span></span>|
|<span data-ttu-id="15b9a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15b9a-117">Application</span></span>|<span data-ttu-id="15b9a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b9a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15b9a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15b9a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="15b9a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15b9a-120">Request headers</span></span>
|<span data-ttu-id="15b9a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15b9a-121">Header</span></span>|<span data-ttu-id="15b9a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15b9a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15b9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15b9a-123">Authorization</span></span>|<span data-ttu-id="15b9a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="15b9a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15b9a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15b9a-125">Accept</span></span>|<span data-ttu-id="15b9a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15b9a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15b9a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15b9a-127">Request body</span></span>
<span data-ttu-id="15b9a-128">В тексте запроса укажите представление JSON для объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="15b9a-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="15b9a-129">В следующей таблице показаны свойства, которые необходимы для создания [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="15b9a-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="15b9a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15b9a-130">Property</span></span>|<span data-ttu-id="15b9a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15b9a-131">Type</span></span>|<span data-ttu-id="15b9a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15b9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15b9a-133">id</span><span class="sxs-lookup"><span data-stu-id="15b9a-133">id</span></span>|<span data-ttu-id="15b9a-134">String</span><span class="sxs-lookup"><span data-stu-id="15b9a-134">String</span></span>|<span data-ttu-id="15b9a-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15b9a-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15b9a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="15b9a-136">displayName</span></span>|<span data-ttu-id="15b9a-137">String</span><span class="sxs-lookup"><span data-stu-id="15b9a-137">String</span></span>|<span data-ttu-id="15b9a-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15b9a-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15b9a-139">description</span><span class="sxs-lookup"><span data-stu-id="15b9a-139">description</span></span>|<span data-ttu-id="15b9a-140">String</span><span class="sxs-lookup"><span data-stu-id="15b9a-140">String</span></span>|<span data-ttu-id="15b9a-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15b9a-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15b9a-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="15b9a-142">requiresUserAuthentication</span></span>|<span data-ttu-id="15b9a-143">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-143">Boolean</span></span>|<span data-ttu-id="15b9a-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15b9a-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15b9a-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="15b9a-145">configurationEndpointUrl</span></span>|<span data-ttu-id="15b9a-146">String</span><span class="sxs-lookup"><span data-stu-id="15b9a-146">String</span></span>|<span data-ttu-id="15b9a-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15b9a-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15b9a-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="15b9a-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="15b9a-149">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-149">Boolean</span></span>|<span data-ttu-id="15b9a-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="15b9a-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="15b9a-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15b9a-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15b9a-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="15b9a-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="15b9a-153">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-153">Boolean</span></span>|<span data-ttu-id="15b9a-154">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15b9a-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="15b9a-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="15b9a-155">isDefault</span></span>|<span data-ttu-id="15b9a-156">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-156">Boolean</span></span>|<span data-ttu-id="15b9a-157">Указывает, является ли профиля по умолчанию</span><span class="sxs-lookup"><span data-stu-id="15b9a-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="15b9a-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-158">supervisedModeEnabled</span></span>|<span data-ttu-id="15b9a-159">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-159">Boolean</span></span>|<span data-ttu-id="15b9a-160">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="15b9a-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="15b9a-161">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="15b9a-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="15b9a-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="15b9a-162">supportDepartment</span></span>|<span data-ttu-id="15b9a-163">String</span><span class="sxs-lookup"><span data-stu-id="15b9a-163">String</span></span>|<span data-ttu-id="15b9a-164">Сведения о поддержке отдела</span><span class="sxs-lookup"><span data-stu-id="15b9a-164">Support department information</span></span>|
|<span data-ttu-id="15b9a-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-165">passCodeDisabled</span></span>|<span data-ttu-id="15b9a-166">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-166">Boolean</span></span>|<span data-ttu-id="15b9a-167">Указывает, если область настройки секретный код отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="15b9a-168">isMandatory</span></span>|<span data-ttu-id="15b9a-169">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-169">Boolean</span></span>|<span data-ttu-id="15b9a-170">Указывает, является ли обязательных профилей</span><span class="sxs-lookup"><span data-stu-id="15b9a-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="15b9a-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-171">locationDisabled</span></span>|<span data-ttu-id="15b9a-172">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-172">Boolean</span></span>|<span data-ttu-id="15b9a-173">Указывает, если область настройки расположения службы отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="15b9a-174">supportPhoneNumber</span></span>|<span data-ttu-id="15b9a-175">String</span><span class="sxs-lookup"><span data-stu-id="15b9a-175">String</span></span>|<span data-ttu-id="15b9a-176">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="15b9a-176">Support phone number</span></span>|
|<span data-ttu-id="15b9a-177">iTunesPairingMode.</span><span class="sxs-lookup"><span data-stu-id="15b9a-177">iTunesPairingMode</span></span>|<span data-ttu-id="15b9a-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="15b9a-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="15b9a-179">Указывает iTunes, режим связывания.</span><span class="sxs-lookup"><span data-stu-id="15b9a-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="15b9a-180">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="15b9a-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="15b9a-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-181">profileRemovalDisabled</span></span>|<span data-ttu-id="15b9a-182">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-182">Boolean</span></span>|<span data-ttu-id="15b9a-183">Указывает, если параметр удаления профиль отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="15b9a-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="15b9a-184">managementCertificates</span></span>|<span data-ttu-id="15b9a-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15b9a-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="15b9a-186">Управление сертификатами для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="15b9a-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="15b9a-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="15b9a-187">restoreBlocked</span></span>|<span data-ttu-id="15b9a-188">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-188">Boolean</span></span>|<span data-ttu-id="15b9a-189">Указывает, если область настройки восстановления блокируется</span><span class="sxs-lookup"><span data-stu-id="15b9a-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="15b9a-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="15b9a-191">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-191">Boolean</span></span>|<span data-ttu-id="15b9a-192">Указывает, если отключено восстановление из Android (en)</span><span class="sxs-lookup"><span data-stu-id="15b9a-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="15b9a-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-193">appleIdDisabled</span></span>|<span data-ttu-id="15b9a-194">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-194">Boolean</span></span>|<span data-ttu-id="15b9a-195">Указывает, если область настройки идентификатор Apple отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="15b9a-197">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-197">Boolean</span></span>|<span data-ttu-id="15b9a-198">Указывает, если отключено «Сроками и условиями» область настройки</span><span class="sxs-lookup"><span data-stu-id="15b9a-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-199">touchIdDisabled</span></span>|<span data-ttu-id="15b9a-200">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-200">Boolean</span></span>|<span data-ttu-id="15b9a-201">Указывает, если область настройки идентификатор сенсорного ввода отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-202">applePayDisabled</span></span>|<span data-ttu-id="15b9a-203">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-203">Boolean</span></span>|<span data-ttu-id="15b9a-204">Указывает, если область настройки оплаты Apple отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-205">zoomDisabled</span></span>|<span data-ttu-id="15b9a-206">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-206">Boolean</span></span>|<span data-ttu-id="15b9a-207">Указывает, если область настройки масштаба отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-208">siriDisabled</span></span>|<span data-ttu-id="15b9a-209">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-209">Boolean</span></span>|<span data-ttu-id="15b9a-210">Указывает, если область настроек siri отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-211">diagnosticsDisabled</span></span>|<span data-ttu-id="15b9a-212">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-212">Boolean</span></span>|<span data-ttu-id="15b9a-213">Указывает, если область настройки диагностики отключен</span><span class="sxs-lookup"><span data-stu-id="15b9a-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="15b9a-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="15b9a-215">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-215">Boolean</span></span>|<span data-ttu-id="15b9a-216">Указывает, отключена при регистрации Mac OS</span><span class="sxs-lookup"><span data-stu-id="15b9a-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="15b9a-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="15b9a-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="15b9a-218">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-218">Boolean</span></span>|<span data-ttu-id="15b9a-219">Указывает, если отключено хранилище файлов Mac OS</span><span class="sxs-lookup"><span data-stu-id="15b9a-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="15b9a-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="15b9a-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="15b9a-221">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-221">Boolean</span></span>|<span data-ttu-id="15b9a-222">Указывает, если устройство необходимо подождать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="15b9a-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="15b9a-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="15b9a-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="15b9a-224">Int32</span><span class="sxs-lookup"><span data-stu-id="15b9a-224">Int32</span></span>|<span data-ttu-id="15b9a-225">Это указывает максимальное количество пользователей, которые могут использовать общие iPad.</span><span class="sxs-lookup"><span data-stu-id="15b9a-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="15b9a-226">Применим только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="15b9a-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="15b9a-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="15b9a-227">enableSharedIPad</span></span>|<span data-ttu-id="15b9a-228">Логический</span><span class="sxs-lookup"><span data-stu-id="15b9a-228">Boolean</span></span>|<span data-ttu-id="15b9a-229">Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии.</span><span class="sxs-lookup"><span data-stu-id="15b9a-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="15b9a-230">Применим только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="15b9a-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="15b9a-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="15b9a-231">Response</span></span>
<span data-ttu-id="15b9a-232">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15b9a-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15b9a-233">Пример</span><span class="sxs-lookup"><span data-stu-id="15b9a-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="15b9a-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="15b9a-234">Request</span></span>
<span data-ttu-id="15b9a-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15b9a-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
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

### <a name="response"></a><span data-ttu-id="15b9a-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="15b9a-236">Response</span></span>
<span data-ttu-id="15b9a-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="15b9a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




