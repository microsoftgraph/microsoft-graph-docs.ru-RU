---
title: Обновление depEnrollmentProfile
description: Обновление свойств объекта depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 152aef9e9351a522f667cbb6c9715e54e2c8eec5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076927"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="d656e-103">Обновление depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d656e-103">Update depEnrollmentProfile</span></span>

<span data-ttu-id="d656e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d656e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d656e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d656e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d656e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d656e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d656e-107">Обновление свойств объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d656e-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d656e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d656e-108">Prerequisites</span></span>
<span data-ttu-id="d656e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d656e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d656e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d656e-111">Permission type</span></span>|<span data-ttu-id="d656e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d656e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d656e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d656e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d656e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d656e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d656e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d656e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d656e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d656e-116">Not supported.</span></span>|
|<span data-ttu-id="d656e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d656e-117">Application</span></span>|<span data-ttu-id="d656e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d656e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d656e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d656e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="d656e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d656e-120">Request headers</span></span>
|<span data-ttu-id="d656e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d656e-121">Header</span></span>|<span data-ttu-id="d656e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d656e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d656e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d656e-123">Authorization</span></span>|<span data-ttu-id="d656e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d656e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d656e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d656e-125">Accept</span></span>|<span data-ttu-id="d656e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d656e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d656e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d656e-127">Request body</span></span>
<span data-ttu-id="d656e-128">В тексте запроса добавьте представление объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d656e-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d656e-129">В следующей таблице приведены свойства, необходимые при создании [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d656e-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="d656e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d656e-130">Property</span></span>|<span data-ttu-id="d656e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d656e-131">Type</span></span>|<span data-ttu-id="d656e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d656e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d656e-133">id</span><span class="sxs-lookup"><span data-stu-id="d656e-133">id</span></span>|<span data-ttu-id="d656e-134">String</span><span class="sxs-lookup"><span data-stu-id="d656e-134">String</span></span>|<span data-ttu-id="d656e-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d656e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d656e-136">displayName</span></span>|<span data-ttu-id="d656e-137">String</span><span class="sxs-lookup"><span data-stu-id="d656e-137">String</span></span>|<span data-ttu-id="d656e-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d656e-139">description</span><span class="sxs-lookup"><span data-stu-id="d656e-139">description</span></span>|<span data-ttu-id="d656e-140">String</span><span class="sxs-lookup"><span data-stu-id="d656e-140">String</span></span>|<span data-ttu-id="d656e-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d656e-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="d656e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="d656e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-143">Boolean</span></span>|<span data-ttu-id="d656e-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d656e-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="d656e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="d656e-146">String</span><span class="sxs-lookup"><span data-stu-id="d656e-146">String</span></span>|<span data-ttu-id="d656e-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d656e-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d656e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d656e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-149">Boolean</span></span>|<span data-ttu-id="d656e-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="d656e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d656e-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d656e-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="d656e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d656e-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-153">Boolean</span></span>|<span data-ttu-id="d656e-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d656e-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="d656e-155">isDefault</span></span>|<span data-ttu-id="d656e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-156">Boolean</span></span>|<span data-ttu-id="d656e-157">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d656e-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="d656e-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-158">supervisedModeEnabled</span></span>|<span data-ttu-id="d656e-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-159">Boolean</span></span>|<span data-ttu-id="d656e-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="d656e-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d656e-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="d656e-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="d656e-162">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="d656e-162">supportDepartment</span></span>|<span data-ttu-id="d656e-163">String</span><span class="sxs-lookup"><span data-stu-id="d656e-163">String</span></span>|<span data-ttu-id="d656e-164">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="d656e-164">Support department information</span></span>|
|<span data-ttu-id="d656e-165">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-165">passCodeDisabled</span></span>|<span data-ttu-id="d656e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-166">Boolean</span></span>|<span data-ttu-id="d656e-167">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="d656e-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d656e-168">isMandatory</span></span>|<span data-ttu-id="d656e-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-169">Boolean</span></span>|<span data-ttu-id="d656e-170">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="d656e-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="d656e-171">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-171">locationDisabled</span></span>|<span data-ttu-id="d656e-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-172">Boolean</span></span>|<span data-ttu-id="d656e-173">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="d656e-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-174">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="d656e-174">supportPhoneNumber</span></span>|<span data-ttu-id="d656e-175">String</span><span class="sxs-lookup"><span data-stu-id="d656e-175">String</span></span>|<span data-ttu-id="d656e-176">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="d656e-176">Support phone number</span></span>|
|<span data-ttu-id="d656e-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d656e-177">iTunesPairingMode</span></span>|<span data-ttu-id="d656e-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="d656e-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="d656e-179">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="d656e-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="d656e-180">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="d656e-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="d656e-181">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-181">profileRemovalDisabled</span></span>|<span data-ttu-id="d656e-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-182">Boolean</span></span>|<span data-ttu-id="d656e-183">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="d656e-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="d656e-184">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="d656e-184">managementCertificates</span></span>|<span data-ttu-id="d656e-185">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="d656e-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="d656e-186">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="d656e-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="d656e-187">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="d656e-187">restoreBlocked</span></span>|<span data-ttu-id="d656e-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-188">Boolean</span></span>|<span data-ttu-id="d656e-189">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="d656e-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="d656e-190">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="d656e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-191">Boolean</span></span>|<span data-ttu-id="d656e-192">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="d656e-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="d656e-193">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-193">appleIdDisabled</span></span>|<span data-ttu-id="d656e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-194">Boolean</span></span>|<span data-ttu-id="d656e-195">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="d656e-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-196">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d656e-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-197">Boolean</span></span>|<span data-ttu-id="d656e-198">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="d656e-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-199">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-199">touchIdDisabled</span></span>|<span data-ttu-id="d656e-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-200">Boolean</span></span>|<span data-ttu-id="d656e-201">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="d656e-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-202">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-202">applePayDisabled</span></span>|<span data-ttu-id="d656e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-203">Boolean</span></span>|<span data-ttu-id="d656e-204">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="d656e-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-205">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-205">zoomDisabled</span></span>|<span data-ttu-id="d656e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-206">Boolean</span></span>|<span data-ttu-id="d656e-207">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="d656e-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-208">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-208">siriDisabled</span></span>|<span data-ttu-id="d656e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-209">Boolean</span></span>|<span data-ttu-id="d656e-210">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="d656e-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-211">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-211">diagnosticsDisabled</span></span>|<span data-ttu-id="d656e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-212">Boolean</span></span>|<span data-ttu-id="d656e-213">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="d656e-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="d656e-214">макосрегистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="d656e-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-215">Boolean</span></span>|<span data-ttu-id="d656e-216">Указывает, отключена ли регистрация Mac OS</span><span class="sxs-lookup"><span data-stu-id="d656e-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="d656e-217">макосфилеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="d656e-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="d656e-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-218">Boolean</span></span>|<span data-ttu-id="d656e-219">Указывает, отключено ли хранилище файлов Mac OS</span><span class="sxs-lookup"><span data-stu-id="d656e-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="d656e-220">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="d656e-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="d656e-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-221">Boolean</span></span>|<span data-ttu-id="d656e-222">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="d656e-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="d656e-223">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="d656e-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="d656e-224">Int32</span><span class="sxs-lookup"><span data-stu-id="d656e-224">Int32</span></span>|<span data-ttu-id="d656e-225">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="d656e-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="d656e-226">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="d656e-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="d656e-227">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="d656e-227">enableSharedIPad</span></span>|<span data-ttu-id="d656e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="d656e-228">Boolean</span></span>|<span data-ttu-id="d656e-229">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="d656e-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="d656e-230">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="d656e-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="d656e-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="d656e-231">Response</span></span>
<span data-ttu-id="d656e-232">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d656e-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d656e-233">Пример</span><span class="sxs-lookup"><span data-stu-id="d656e-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="d656e-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="d656e-234">Request</span></span>
<span data-ttu-id="d656e-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d656e-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d656e-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="d656e-236">Response</span></span>
<span data-ttu-id="d656e-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d656e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






