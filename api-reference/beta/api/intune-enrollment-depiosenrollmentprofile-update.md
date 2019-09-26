---
title: Обновление Депиосенроллментпрофиле
description: Обновление свойств объекта Депиосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b46a35095ed46f257a528d2e661c3311b711d08
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187879"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="96964-103">Обновление Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="96964-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="96964-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96964-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96964-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96964-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96964-106">Обновление свойств объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="96964-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96964-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96964-107">Prerequisites</span></span>
<span data-ttu-id="96964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96964-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96964-110">Permission type</span></span>|<span data-ttu-id="96964-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96964-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96964-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96964-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96964-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96964-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="96964-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96964-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96964-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96964-115">Not supported.</span></span>|
|<span data-ttu-id="96964-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96964-116">Application</span></span>|<span data-ttu-id="96964-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96964-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96964-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96964-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="96964-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96964-119">Request headers</span></span>
|<span data-ttu-id="96964-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96964-120">Header</span></span>|<span data-ttu-id="96964-121">Значение</span><span class="sxs-lookup"><span data-stu-id="96964-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96964-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96964-122">Authorization</span></span>|<span data-ttu-id="96964-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96964-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96964-124">Accept</span><span class="sxs-lookup"><span data-stu-id="96964-124">Accept</span></span>|<span data-ttu-id="96964-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96964-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96964-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96964-126">Request body</span></span>
<span data-ttu-id="96964-127">В тексте запроса добавьте представление объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96964-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="96964-128">В следующей таблице приведены свойства, необходимые при создании [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="96964-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="96964-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="96964-129">Property</span></span>|<span data-ttu-id="96964-130">Тип</span><span class="sxs-lookup"><span data-stu-id="96964-130">Type</span></span>|<span data-ttu-id="96964-131">Описание</span><span class="sxs-lookup"><span data-stu-id="96964-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96964-132">id</span><span class="sxs-lookup"><span data-stu-id="96964-132">id</span></span>|<span data-ttu-id="96964-133">String</span><span class="sxs-lookup"><span data-stu-id="96964-133">String</span></span>|<span data-ttu-id="96964-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="96964-135">displayName</span><span class="sxs-lookup"><span data-stu-id="96964-135">displayName</span></span>|<span data-ttu-id="96964-136">Строка</span><span class="sxs-lookup"><span data-stu-id="96964-136">String</span></span>|<span data-ttu-id="96964-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="96964-138">description</span><span class="sxs-lookup"><span data-stu-id="96964-138">description</span></span>|<span data-ttu-id="96964-139">String</span><span class="sxs-lookup"><span data-stu-id="96964-139">String</span></span>|<span data-ttu-id="96964-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="96964-141">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="96964-141">requiresUserAuthentication</span></span>|<span data-ttu-id="96964-142">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-142">Boolean</span></span>|<span data-ttu-id="96964-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="96964-144">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="96964-144">configurationEndpointUrl</span></span>|<span data-ttu-id="96964-145">String.</span><span class="sxs-lookup"><span data-stu-id="96964-145">String</span></span>|<span data-ttu-id="96964-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="96964-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="96964-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="96964-148">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-148">Boolean</span></span>|<span data-ttu-id="96964-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="96964-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="96964-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="96964-151">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="96964-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="96964-152">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-152">Boolean</span></span>|<span data-ttu-id="96964-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="96964-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="96964-154">isDefault</span></span>|<span data-ttu-id="96964-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="96964-155">Boolean</span></span>|<span data-ttu-id="96964-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-157">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="96964-157">supervisedModeEnabled</span></span>|<span data-ttu-id="96964-158">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-158">Boolean</span></span>|<span data-ttu-id="96964-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="96964-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="96964-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="96964-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="96964-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-162">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="96964-162">supportDepartment</span></span>|<span data-ttu-id="96964-163">String.</span><span class="sxs-lookup"><span data-stu-id="96964-163">String</span></span>|<span data-ttu-id="96964-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-165">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-165">passCodeDisabled</span></span>|<span data-ttu-id="96964-166">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-166">Boolean</span></span>|<span data-ttu-id="96964-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="96964-168">isMandatory</span></span>|<span data-ttu-id="96964-169">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-169">Boolean</span></span>|<span data-ttu-id="96964-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-171">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-171">locationDisabled</span></span>|<span data-ttu-id="96964-172">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-172">Boolean</span></span>|<span data-ttu-id="96964-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-174">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="96964-174">supportPhoneNumber</span></span>|<span data-ttu-id="96964-175">String.</span><span class="sxs-lookup"><span data-stu-id="96964-175">String</span></span>|<span data-ttu-id="96964-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-177">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-177">profileRemovalDisabled</span></span>|<span data-ttu-id="96964-178">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-178">Boolean</span></span>|<span data-ttu-id="96964-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-180">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="96964-180">restoreBlocked</span></span>|<span data-ttu-id="96964-181">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-181">Boolean</span></span>|<span data-ttu-id="96964-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-183">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-183">appleIdDisabled</span></span>|<span data-ttu-id="96964-184">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-184">Boolean</span></span>|<span data-ttu-id="96964-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-186">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="96964-187">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-187">Boolean</span></span>|<span data-ttu-id="96964-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-189">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-189">touchIdDisabled</span></span>|<span data-ttu-id="96964-190">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-190">Boolean</span></span>|<span data-ttu-id="96964-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-192">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-192">applePayDisabled</span></span>|<span data-ttu-id="96964-193">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-193">Boolean</span></span>|<span data-ttu-id="96964-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-195">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-195">zoomDisabled</span></span>|<span data-ttu-id="96964-196">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-196">Boolean</span></span>|<span data-ttu-id="96964-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-198">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-198">siriDisabled</span></span>|<span data-ttu-id="96964-199">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-199">Boolean</span></span>|<span data-ttu-id="96964-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-201">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-201">diagnosticsDisabled</span></span>|<span data-ttu-id="96964-202">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-202">Boolean</span></span>|<span data-ttu-id="96964-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-204">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="96964-205">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-205">Boolean</span></span>|<span data-ttu-id="96964-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-207">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-207">privacyPaneDisabled</span></span>|<span data-ttu-id="96964-208">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-208">Boolean</span></span>|<span data-ttu-id="96964-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-210">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="96964-211">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-211">Boolean</span></span>|<span data-ttu-id="96964-212">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-213">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="96964-213">deviceNameTemplate</span></span>|<span data-ttu-id="96964-214">String.</span><span class="sxs-lookup"><span data-stu-id="96964-214">String</span></span>|<span data-ttu-id="96964-215">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="96964-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="96964-216">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96964-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="96964-217">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="96964-217">iTunesPairingMode</span></span>|<span data-ttu-id="96964-218">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="96964-218">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="96964-219">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="96964-219">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="96964-220">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="96964-220">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="96964-221">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="96964-221">managementCertificates</span></span>|<span data-ttu-id="96964-222">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="96964-222">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="96964-223">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="96964-223">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="96964-224">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-224">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="96964-225">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-225">Boolean</span></span>|<span data-ttu-id="96964-226">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="96964-226">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="96964-227">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="96964-227">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="96964-228">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-228">Boolean</span></span>|<span data-ttu-id="96964-229">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="96964-229">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="96964-230">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="96964-230">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="96964-231">Int32</span><span class="sxs-lookup"><span data-stu-id="96964-231">Int32</span></span>|<span data-ttu-id="96964-232">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="96964-232">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="96964-233">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="96964-233">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="96964-234">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="96964-234">enableSharedIPad</span></span>|<span data-ttu-id="96964-235">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-235">Boolean</span></span>|<span data-ttu-id="96964-236">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="96964-236">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="96964-237">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="96964-237">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="96964-238">компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="96964-238">companyPortalVppTokenId</span></span>|<span data-ttu-id="96964-239">String.</span><span class="sxs-lookup"><span data-stu-id="96964-239">String</span></span>|<span data-ttu-id="96964-240">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="96964-240">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="96964-241">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="96964-241">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="96964-242">енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="96964-242">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="96964-243">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-243">Boolean</span></span>|<span data-ttu-id="96964-244">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="96964-244">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="96964-245">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="96964-245">Default is false.</span></span> <span data-ttu-id="96964-246">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="96964-246">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="96964-247">хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-247">homeButtonScreenDisabled</span></span>|<span data-ttu-id="96964-248">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-248">Boolean</span></span>|<span data-ttu-id="96964-249">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="96964-249">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="96964-250">имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-250">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="96964-251">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-251">Boolean</span></span>|<span data-ttu-id="96964-252">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="96964-252">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="96964-253">онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-253">onBoardingScreenDisabled</span></span>|<span data-ttu-id="96964-254">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-254">Boolean</span></span>|<span data-ttu-id="96964-255">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="96964-255">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="96964-256">симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="96964-257">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-257">Boolean</span></span>|<span data-ttu-id="96964-258">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="96964-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="96964-259">софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="96964-260">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-260">Boolean</span></span>|<span data-ttu-id="96964-261">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="96964-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="96964-262">ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="96964-263">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-263">Boolean</span></span>|<span data-ttu-id="96964-264">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="96964-264">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="96964-265">аппеаранцескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-265">appearanceScreenDisabled</span></span>|<span data-ttu-id="96964-266">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-266">Boolean</span></span>|<span data-ttu-id="96964-267">Указывает, отключен ли экран Апперанце</span><span class="sxs-lookup"><span data-stu-id="96964-267">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="96964-268">експресслангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-268">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="96964-269">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-269">Boolean</span></span>|<span data-ttu-id="96964-270">Указывает, отключен ли экран Express Language</span><span class="sxs-lookup"><span data-stu-id="96964-270">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="96964-271">преферредлангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-271">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="96964-272">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-272">Boolean</span></span>|<span data-ttu-id="96964-273">Указывает, отключен ли предпочтительный экран языка</span><span class="sxs-lookup"><span data-stu-id="96964-273">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="96964-274">девицетодевицемигратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-274">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="96964-275">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-275">Boolean</span></span>|<span data-ttu-id="96964-276">Указывает, отключена ли миграция устройств для устройств</span><span class="sxs-lookup"><span data-stu-id="96964-276">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="96964-277">велкомескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="96964-277">welcomeScreenDisabled</span></span>|<span data-ttu-id="96964-278">Boolean.</span><span class="sxs-lookup"><span data-stu-id="96964-278">Boolean</span></span>|<span data-ttu-id="96964-279">Указывает, отключен ли экран Векломе</span><span class="sxs-lookup"><span data-stu-id="96964-279">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="96964-280">Отклик</span><span class="sxs-lookup"><span data-stu-id="96964-280">Response</span></span>
<span data-ttu-id="96964-281">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96964-281">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96964-282">Пример</span><span class="sxs-lookup"><span data-stu-id="96964-282">Example</span></span>

### <a name="request"></a><span data-ttu-id="96964-283">Запрос</span><span class="sxs-lookup"><span data-stu-id="96964-283">Request</span></span>
<span data-ttu-id="96964-284">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96964-284">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1992

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
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
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
  "welcomeScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="96964-285">Отклик</span><span class="sxs-lookup"><span data-stu-id="96964-285">Response</span></span>
<span data-ttu-id="96964-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96964-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2041

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
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
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
  "welcomeScreenDisabled": true
}
```




