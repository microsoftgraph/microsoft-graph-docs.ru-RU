---
title: Создание depEnrollmentProfile
description: Создание нового объекта depEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ce46c8ff178b62f7b99f7bf454ccd29689fac1e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533991"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="23651-103">Создание depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="23651-103">Create depEnrollmentProfile</span></span>

> <span data-ttu-id="23651-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23651-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23651-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23651-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23651-106">Создание нового объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="23651-106">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23651-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23651-107">Prerequisites</span></span>
<span data-ttu-id="23651-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23651-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23651-110">Permission type</span></span>|<span data-ttu-id="23651-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23651-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23651-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23651-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23651-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23651-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23651-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23651-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23651-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23651-115">Not supported.</span></span>|
|<span data-ttu-id="23651-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23651-116">Application</span></span>|<span data-ttu-id="23651-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23651-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23651-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23651-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="23651-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23651-119">Request headers</span></span>
|<span data-ttu-id="23651-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23651-120">Header</span></span>|<span data-ttu-id="23651-121">Значение</span><span class="sxs-lookup"><span data-stu-id="23651-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23651-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23651-122">Authorization</span></span>|<span data-ttu-id="23651-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23651-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23651-124">Accept</span><span class="sxs-lookup"><span data-stu-id="23651-124">Accept</span></span>|<span data-ttu-id="23651-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23651-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23651-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23651-126">Request body</span></span>
<span data-ttu-id="23651-127">В тексте запроса добавьте представление объекта depEnrollmentProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23651-127">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="23651-128">В следующей таблице приведены свойства, необходимые при создании depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="23651-128">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="23651-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="23651-129">Property</span></span>|<span data-ttu-id="23651-130">Тип</span><span class="sxs-lookup"><span data-stu-id="23651-130">Type</span></span>|<span data-ttu-id="23651-131">Описание</span><span class="sxs-lookup"><span data-stu-id="23651-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23651-132">id</span><span class="sxs-lookup"><span data-stu-id="23651-132">id</span></span>|<span data-ttu-id="23651-133">Строка</span><span class="sxs-lookup"><span data-stu-id="23651-133">String</span></span>|<span data-ttu-id="23651-134">GUID объекта, наСледуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="23651-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="23651-135">displayName</span><span class="sxs-lookup"><span data-stu-id="23651-135">displayName</span></span>|<span data-ttu-id="23651-136">String</span><span class="sxs-lookup"><span data-stu-id="23651-136">String</span></span>|<span data-ttu-id="23651-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="23651-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="23651-138">description</span><span class="sxs-lookup"><span data-stu-id="23651-138">description</span></span>|<span data-ttu-id="23651-139">String</span><span class="sxs-lookup"><span data-stu-id="23651-139">String</span></span>|<span data-ttu-id="23651-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="23651-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="23651-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="23651-141">requiresUserAuthentication</span></span>|<span data-ttu-id="23651-142">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-142">Boolean</span></span>|<span data-ttu-id="23651-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="23651-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="23651-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="23651-144">configurationEndpointUrl</span></span>|<span data-ttu-id="23651-145">String</span><span class="sxs-lookup"><span data-stu-id="23651-145">String</span></span>|<span data-ttu-id="23651-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="23651-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="23651-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="23651-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="23651-148">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-148">Boolean</span></span>|<span data-ttu-id="23651-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="23651-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="23651-150">НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="23651-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="23651-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="23651-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="23651-152">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-152">Boolean</span></span>|<span data-ttu-id="23651-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наСледуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="23651-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="23651-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="23651-154">isDefault</span></span>|<span data-ttu-id="23651-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="23651-155">Boolean</span></span>|<span data-ttu-id="23651-156">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="23651-156">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="23651-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="23651-157">supervisedModeEnabled</span></span>|<span data-ttu-id="23651-158">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-158">Boolean</span></span>|<span data-ttu-id="23651-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="23651-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="23651-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="23651-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="23651-161">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="23651-161">supportDepartment</span></span>|<span data-ttu-id="23651-162">String</span><span class="sxs-lookup"><span data-stu-id="23651-162">String</span></span>|<span data-ttu-id="23651-163">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="23651-163">Support department information</span></span>|
|<span data-ttu-id="23651-164">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-164">passCodeDisabled</span></span>|<span data-ttu-id="23651-165">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-165">Boolean</span></span>|<span data-ttu-id="23651-166">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="23651-166">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="23651-167">Обязательный</span><span class="sxs-lookup"><span data-stu-id="23651-167">isMandatory</span></span>|<span data-ttu-id="23651-168">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-168">Boolean</span></span>|<span data-ttu-id="23651-169">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="23651-169">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="23651-170">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-170">locationDisabled</span></span>|<span data-ttu-id="23651-171">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-171">Boolean</span></span>|<span data-ttu-id="23651-172">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="23651-172">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="23651-173">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="23651-173">supportPhoneNumber</span></span>|<span data-ttu-id="23651-174">String</span><span class="sxs-lookup"><span data-stu-id="23651-174">String</span></span>|<span data-ttu-id="23651-175">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="23651-175">Support phone number</span></span>|
|<span data-ttu-id="23651-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="23651-176">iTunesPairingMode</span></span>|<span data-ttu-id="23651-177">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="23651-177">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="23651-178">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="23651-178">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="23651-179">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="23651-179">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="23651-180">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-180">profileRemovalDisabled</span></span>|<span data-ttu-id="23651-181">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-181">Boolean</span></span>|<span data-ttu-id="23651-182">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="23651-182">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="23651-183">Манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="23651-183">managementCertificates</span></span>|<span data-ttu-id="23651-184">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="23651-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="23651-185">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="23651-185">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="23651-186">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="23651-186">restoreBlocked</span></span>|<span data-ttu-id="23651-187">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-187">Boolean</span></span>|<span data-ttu-id="23651-188">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="23651-188">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="23651-189">Ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-189">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="23651-190">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-190">Boolean</span></span>|<span data-ttu-id="23651-191">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="23651-191">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="23651-192">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-192">appleIdDisabled</span></span>|<span data-ttu-id="23651-193">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-193">Boolean</span></span>|<span data-ttu-id="23651-194">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="23651-194">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="23651-195">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-195">termsAndConditionsDisabled</span></span>|<span data-ttu-id="23651-196">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-196">Boolean</span></span>|<span data-ttu-id="23651-197">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="23651-197">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="23651-198">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-198">touchIdDisabled</span></span>|<span data-ttu-id="23651-199">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-199">Boolean</span></span>|<span data-ttu-id="23651-200">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="23651-200">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="23651-201">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-201">applePayDisabled</span></span>|<span data-ttu-id="23651-202">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-202">Boolean</span></span>|<span data-ttu-id="23651-203">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="23651-203">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="23651-204">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-204">zoomDisabled</span></span>|<span data-ttu-id="23651-205">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-205">Boolean</span></span>|<span data-ttu-id="23651-206">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="23651-206">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="23651-207">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-207">siriDisabled</span></span>|<span data-ttu-id="23651-208">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-208">Boolean</span></span>|<span data-ttu-id="23651-209">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="23651-209">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="23651-210">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-210">diagnosticsDisabled</span></span>|<span data-ttu-id="23651-211">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-211">Boolean</span></span>|<span data-ttu-id="23651-212">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="23651-212">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="23651-213">Макосрегистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-213">macOSRegistrationDisabled</span></span>|<span data-ttu-id="23651-214">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-214">Boolean</span></span>|<span data-ttu-id="23651-215">Указывает, отключена ли регистрация Mac OS</span><span class="sxs-lookup"><span data-stu-id="23651-215">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="23651-216">Макосфилеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="23651-216">macOSFileVaultDisabled</span></span>|<span data-ttu-id="23651-217">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-217">Boolean</span></span>|<span data-ttu-id="23651-218">Указывает, отключено ли хранилище файлов Mac OS</span><span class="sxs-lookup"><span data-stu-id="23651-218">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="23651-219">Аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="23651-219">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="23651-220">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-220">Boolean</span></span>|<span data-ttu-id="23651-221">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="23651-221">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="23651-222">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="23651-222">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="23651-223">Int32</span><span class="sxs-lookup"><span data-stu-id="23651-223">Int32</span></span>|<span data-ttu-id="23651-224">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="23651-224">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="23651-225">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="23651-225">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="23651-226">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="23651-226">enableSharedIPad</span></span>|<span data-ttu-id="23651-227">Логический</span><span class="sxs-lookup"><span data-stu-id="23651-227">Boolean</span></span>|<span data-ttu-id="23651-228">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="23651-228">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="23651-229">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="23651-229">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="23651-230">Ответ</span><span class="sxs-lookup"><span data-stu-id="23651-230">Response</span></span>
<span data-ttu-id="23651-231">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23651-231">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23651-232">Пример</span><span class="sxs-lookup"><span data-stu-id="23651-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="23651-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="23651-233">Request</span></span>
<span data-ttu-id="23651-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23651-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="23651-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="23651-235">Response</span></span>
<span data-ttu-id="23651-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23651-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





