---
title: Создание depEnrollmentProfile
description: Создание нового объекта depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 076bb1e878b26d733ab3309e9bb4c1f1bf46678d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202229"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="93394-103">Создание depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="93394-103">Create depEnrollmentProfile</span></span>

<span data-ttu-id="93394-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93394-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93394-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93394-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93394-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93394-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93394-107">Создание нового объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="93394-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93394-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93394-108">Prerequisites</span></span>
<span data-ttu-id="93394-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93394-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93394-111">Permission type</span></span>|<span data-ttu-id="93394-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93394-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93394-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93394-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93394-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93394-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93394-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93394-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93394-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93394-116">Not supported.</span></span>|
|<span data-ttu-id="93394-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="93394-117">Application</span></span>|<span data-ttu-id="93394-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93394-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93394-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93394-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="93394-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93394-120">Request headers</span></span>
|<span data-ttu-id="93394-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93394-121">Header</span></span>|<span data-ttu-id="93394-122">Значение</span><span class="sxs-lookup"><span data-stu-id="93394-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93394-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93394-123">Authorization</span></span>|<span data-ttu-id="93394-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93394-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93394-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93394-125">Accept</span></span>|<span data-ttu-id="93394-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93394-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93394-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93394-127">Request body</span></span>
<span data-ttu-id="93394-128">В тексте запроса добавьте представление объекта depEnrollmentProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93394-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="93394-129">В следующей таблице приведены свойства, необходимые при создании depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="93394-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="93394-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="93394-130">Property</span></span>|<span data-ttu-id="93394-131">Тип</span><span class="sxs-lookup"><span data-stu-id="93394-131">Type</span></span>|<span data-ttu-id="93394-132">Описание</span><span class="sxs-lookup"><span data-stu-id="93394-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93394-133">id</span><span class="sxs-lookup"><span data-stu-id="93394-133">id</span></span>|<span data-ttu-id="93394-134">String</span><span class="sxs-lookup"><span data-stu-id="93394-134">String</span></span>|<span data-ttu-id="93394-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93394-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="93394-136">displayName</span><span class="sxs-lookup"><span data-stu-id="93394-136">displayName</span></span>|<span data-ttu-id="93394-137">String</span><span class="sxs-lookup"><span data-stu-id="93394-137">String</span></span>|<span data-ttu-id="93394-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93394-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="93394-139">description</span><span class="sxs-lookup"><span data-stu-id="93394-139">description</span></span>|<span data-ttu-id="93394-140">String</span><span class="sxs-lookup"><span data-stu-id="93394-140">String</span></span>|<span data-ttu-id="93394-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93394-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="93394-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="93394-142">requiresUserAuthentication</span></span>|<span data-ttu-id="93394-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-143">Boolean</span></span>|<span data-ttu-id="93394-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93394-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="93394-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="93394-145">configurationEndpointUrl</span></span>|<span data-ttu-id="93394-146">String</span><span class="sxs-lookup"><span data-stu-id="93394-146">String</span></span>|<span data-ttu-id="93394-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93394-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="93394-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="93394-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="93394-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-149">Boolean</span></span>|<span data-ttu-id="93394-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="93394-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="93394-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93394-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="93394-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="93394-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="93394-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-153">Boolean</span></span>|<span data-ttu-id="93394-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93394-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="93394-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="93394-155">isDefault</span></span>|<span data-ttu-id="93394-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-156">Boolean</span></span>|<span data-ttu-id="93394-157">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="93394-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="93394-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="93394-158">supervisedModeEnabled</span></span>|<span data-ttu-id="93394-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-159">Boolean</span></span>|<span data-ttu-id="93394-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="93394-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="93394-161"> https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="93394-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="93394-162">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="93394-162">supportDepartment</span></span>|<span data-ttu-id="93394-163">String</span><span class="sxs-lookup"><span data-stu-id="93394-163">String</span></span>|<span data-ttu-id="93394-164">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="93394-164">Support department information</span></span>|
|<span data-ttu-id="93394-165">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-165">passCodeDisabled</span></span>|<span data-ttu-id="93394-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-166">Boolean</span></span>|<span data-ttu-id="93394-167">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="93394-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="93394-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="93394-168">isMandatory</span></span>|<span data-ttu-id="93394-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-169">Boolean</span></span>|<span data-ttu-id="93394-170">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="93394-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="93394-171">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-171">locationDisabled</span></span>|<span data-ttu-id="93394-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-172">Boolean</span></span>|<span data-ttu-id="93394-173">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="93394-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="93394-174">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="93394-174">supportPhoneNumber</span></span>|<span data-ttu-id="93394-175">String</span><span class="sxs-lookup"><span data-stu-id="93394-175">String</span></span>|<span data-ttu-id="93394-176">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="93394-176">Support phone number</span></span>|
|<span data-ttu-id="93394-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="93394-177">iTunesPairingMode</span></span>|<span data-ttu-id="93394-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="93394-178">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="93394-179">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="93394-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="93394-180">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="93394-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="93394-181">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-181">profileRemovalDisabled</span></span>|<span data-ttu-id="93394-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-182">Boolean</span></span>|<span data-ttu-id="93394-183">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="93394-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="93394-184">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="93394-184">managementCertificates</span></span>|<span data-ttu-id="93394-185">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="93394-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="93394-186">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="93394-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="93394-187">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="93394-187">restoreBlocked</span></span>|<span data-ttu-id="93394-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-188">Boolean</span></span>|<span data-ttu-id="93394-189">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="93394-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="93394-190">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="93394-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-191">Boolean</span></span>|<span data-ttu-id="93394-192">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="93394-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="93394-193">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-193">appleIdDisabled</span></span>|<span data-ttu-id="93394-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-194">Boolean</span></span>|<span data-ttu-id="93394-195">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="93394-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="93394-196">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="93394-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-197">Boolean</span></span>|<span data-ttu-id="93394-198">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="93394-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="93394-199">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-199">touchIdDisabled</span></span>|<span data-ttu-id="93394-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-200">Boolean</span></span>|<span data-ttu-id="93394-201">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="93394-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="93394-202">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-202">applePayDisabled</span></span>|<span data-ttu-id="93394-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-203">Boolean</span></span>|<span data-ttu-id="93394-204">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="93394-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="93394-205">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-205">zoomDisabled</span></span>|<span data-ttu-id="93394-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-206">Boolean</span></span>|<span data-ttu-id="93394-207">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="93394-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="93394-208">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-208">siriDisabled</span></span>|<span data-ttu-id="93394-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-209">Boolean</span></span>|<span data-ttu-id="93394-210">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="93394-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="93394-211">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-211">diagnosticsDisabled</span></span>|<span data-ttu-id="93394-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-212">Boolean</span></span>|<span data-ttu-id="93394-213">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="93394-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="93394-214">макосрегистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="93394-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-215">Boolean</span></span>|<span data-ttu-id="93394-216">Указывает, отключена ли регистрация Mac OS</span><span class="sxs-lookup"><span data-stu-id="93394-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="93394-217">макосфилеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="93394-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="93394-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-218">Boolean</span></span>|<span data-ttu-id="93394-219">Указывает, отключено ли хранилище файлов Mac OS</span><span class="sxs-lookup"><span data-stu-id="93394-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="93394-220">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="93394-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="93394-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-221">Boolean</span></span>|<span data-ttu-id="93394-222">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="93394-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="93394-223">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="93394-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="93394-224">Int32</span><span class="sxs-lookup"><span data-stu-id="93394-224">Int32</span></span>|<span data-ttu-id="93394-225">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="93394-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="93394-226">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="93394-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="93394-227">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="93394-227">enableSharedIPad</span></span>|<span data-ttu-id="93394-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="93394-228">Boolean</span></span>|<span data-ttu-id="93394-229">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="93394-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="93394-230">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="93394-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="93394-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="93394-231">Response</span></span>
<span data-ttu-id="93394-232">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93394-232">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93394-233">Пример</span><span class="sxs-lookup"><span data-stu-id="93394-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="93394-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="93394-234">Request</span></span>
<span data-ttu-id="93394-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93394-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93394-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="93394-236">Response</span></span>
<span data-ttu-id="93394-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93394-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




