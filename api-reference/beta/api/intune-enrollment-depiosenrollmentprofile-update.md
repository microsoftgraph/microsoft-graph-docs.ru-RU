---
title: Обновление Депиосенроллментпрофиле
description: Обновление свойств объекта Депиосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac297f07c319b2f48bb25e492b3f1c78c5336cc6
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943973"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="035a8-103">Обновление Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="035a8-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="035a8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="035a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="035a8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="035a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="035a8-106">Обновление свойств объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="035a8-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="035a8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="035a8-107">Prerequisites</span></span>
<span data-ttu-id="035a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="035a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="035a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="035a8-110">Permission type</span></span>|<span data-ttu-id="035a8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="035a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="035a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="035a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="035a8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="035a8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="035a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="035a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="035a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="035a8-115">Not supported.</span></span>|
|<span data-ttu-id="035a8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="035a8-116">Application</span></span>|<span data-ttu-id="035a8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="035a8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="035a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="035a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="035a8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="035a8-119">Request headers</span></span>
|<span data-ttu-id="035a8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="035a8-120">Header</span></span>|<span data-ttu-id="035a8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="035a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="035a8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="035a8-122">Authorization</span></span>|<span data-ttu-id="035a8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="035a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="035a8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="035a8-124">Accept</span></span>|<span data-ttu-id="035a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="035a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="035a8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="035a8-126">Request body</span></span>
<span data-ttu-id="035a8-127">В тексте запроса добавьте представление объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="035a8-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="035a8-128">В следующей таблице приведены свойства, необходимые при создании [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="035a8-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="035a8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="035a8-129">Property</span></span>|<span data-ttu-id="035a8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="035a8-130">Type</span></span>|<span data-ttu-id="035a8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="035a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="035a8-132">id</span><span class="sxs-lookup"><span data-stu-id="035a8-132">id</span></span>|<span data-ttu-id="035a8-133">String</span><span class="sxs-lookup"><span data-stu-id="035a8-133">String</span></span>|<span data-ttu-id="035a8-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="035a8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="035a8-135">displayName</span></span>|<span data-ttu-id="035a8-136">Строка</span><span class="sxs-lookup"><span data-stu-id="035a8-136">String</span></span>|<span data-ttu-id="035a8-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="035a8-138">description</span><span class="sxs-lookup"><span data-stu-id="035a8-138">description</span></span>|<span data-ttu-id="035a8-139">String</span><span class="sxs-lookup"><span data-stu-id="035a8-139">String</span></span>|<span data-ttu-id="035a8-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="035a8-141">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="035a8-141">requiresUserAuthentication</span></span>|<span data-ttu-id="035a8-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-142">Boolean</span></span>|<span data-ttu-id="035a8-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="035a8-144">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="035a8-144">configurationEndpointUrl</span></span>|<span data-ttu-id="035a8-145">Строка</span><span class="sxs-lookup"><span data-stu-id="035a8-145">String</span></span>|<span data-ttu-id="035a8-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="035a8-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="035a8-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="035a8-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-148">Boolean</span></span>|<span data-ttu-id="035a8-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="035a8-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="035a8-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="035a8-151">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="035a8-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="035a8-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-152">Boolean</span></span>|<span data-ttu-id="035a8-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="035a8-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="035a8-154">isDefault</span></span>|<span data-ttu-id="035a8-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-155">Boolean</span></span>|<span data-ttu-id="035a8-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-157">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-157">supervisedModeEnabled</span></span>|<span data-ttu-id="035a8-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-158">Boolean</span></span>|<span data-ttu-id="035a8-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="035a8-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="035a8-160">Дополнительную https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="035a8-160">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="035a8-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-162">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="035a8-162">supportDepartment</span></span>|<span data-ttu-id="035a8-163">Строка</span><span class="sxs-lookup"><span data-stu-id="035a8-163">String</span></span>|<span data-ttu-id="035a8-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-165">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-165">passCodeDisabled</span></span>|<span data-ttu-id="035a8-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-166">Boolean</span></span>|<span data-ttu-id="035a8-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="035a8-168">isMandatory</span></span>|<span data-ttu-id="035a8-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-169">Boolean</span></span>|<span data-ttu-id="035a8-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-171">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-171">locationDisabled</span></span>|<span data-ttu-id="035a8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-172">Boolean</span></span>|<span data-ttu-id="035a8-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-174">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="035a8-174">supportPhoneNumber</span></span>|<span data-ttu-id="035a8-175">Строка</span><span class="sxs-lookup"><span data-stu-id="035a8-175">String</span></span>|<span data-ttu-id="035a8-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-177">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-177">profileRemovalDisabled</span></span>|<span data-ttu-id="035a8-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-178">Boolean</span></span>|<span data-ttu-id="035a8-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-180">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="035a8-180">restoreBlocked</span></span>|<span data-ttu-id="035a8-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-181">Boolean</span></span>|<span data-ttu-id="035a8-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-183">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-183">appleIdDisabled</span></span>|<span data-ttu-id="035a8-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-184">Boolean</span></span>|<span data-ttu-id="035a8-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-186">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="035a8-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-187">Boolean</span></span>|<span data-ttu-id="035a8-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-189">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-189">touchIdDisabled</span></span>|<span data-ttu-id="035a8-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-190">Boolean</span></span>|<span data-ttu-id="035a8-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-192">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-192">applePayDisabled</span></span>|<span data-ttu-id="035a8-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-193">Boolean</span></span>|<span data-ttu-id="035a8-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-195">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-195">zoomDisabled</span></span>|<span data-ttu-id="035a8-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-196">Boolean</span></span>|<span data-ttu-id="035a8-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-198">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-198">siriDisabled</span></span>|<span data-ttu-id="035a8-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-199">Boolean</span></span>|<span data-ttu-id="035a8-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-201">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-201">diagnosticsDisabled</span></span>|<span data-ttu-id="035a8-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-202">Boolean</span></span>|<span data-ttu-id="035a8-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-204">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="035a8-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-205">Boolean</span></span>|<span data-ttu-id="035a8-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-207">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-207">privacyPaneDisabled</span></span>|<span data-ttu-id="035a8-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-208">Boolean</span></span>|<span data-ttu-id="035a8-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-210">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="035a8-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-211">Boolean</span></span>|<span data-ttu-id="035a8-212">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-213">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="035a8-213">deviceNameTemplate</span></span>|<span data-ttu-id="035a8-214">Строка</span><span class="sxs-lookup"><span data-stu-id="035a8-214">String</span></span>|<span data-ttu-id="035a8-215">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="035a8-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="035a8-216">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-217">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="035a8-217">configurationWebUrl</span></span>|<span data-ttu-id="035a8-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-218">Boolean</span></span>|<span data-ttu-id="035a8-219">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-219">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="035a8-220">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="035a8-220">iTunesPairingMode</span></span>|<span data-ttu-id="035a8-221">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="035a8-221">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="035a8-222">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="035a8-222">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="035a8-223">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="035a8-223">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="035a8-224">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="035a8-224">managementCertificates</span></span>|<span data-ttu-id="035a8-225">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="035a8-225">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="035a8-226">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="035a8-226">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="035a8-227">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-227">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="035a8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-228">Boolean</span></span>|<span data-ttu-id="035a8-229">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="035a8-229">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="035a8-230">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="035a8-230">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="035a8-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-231">Boolean</span></span>|<span data-ttu-id="035a8-232">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="035a8-232">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="035a8-233">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="035a8-233">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="035a8-234">Int32</span><span class="sxs-lookup"><span data-stu-id="035a8-234">Int32</span></span>|<span data-ttu-id="035a8-235">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="035a8-235">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="035a8-236">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="035a8-236">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="035a8-237">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="035a8-237">enableSharedIPad</span></span>|<span data-ttu-id="035a8-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-238">Boolean</span></span>|<span data-ttu-id="035a8-239">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="035a8-239">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="035a8-240">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="035a8-240">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="035a8-241">компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="035a8-241">companyPortalVppTokenId</span></span>|<span data-ttu-id="035a8-242">Строка</span><span class="sxs-lookup"><span data-stu-id="035a8-242">String</span></span>|<span data-ttu-id="035a8-243">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="035a8-243">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="035a8-244">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="035a8-244">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="035a8-245">енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="035a8-245">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="035a8-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-246">Boolean</span></span>|<span data-ttu-id="035a8-247">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="035a8-247">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="035a8-248">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="035a8-248">Default is false.</span></span> <span data-ttu-id="035a8-249">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="035a8-249">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="035a8-250">хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-250">homeButtonScreenDisabled</span></span>|<span data-ttu-id="035a8-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-251">Boolean</span></span>|<span data-ttu-id="035a8-252">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="035a8-252">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="035a8-253">имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-253">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="035a8-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-254">Boolean</span></span>|<span data-ttu-id="035a8-255">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="035a8-255">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="035a8-256">онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-256">onBoardingScreenDisabled</span></span>|<span data-ttu-id="035a8-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-257">Boolean</span></span>|<span data-ttu-id="035a8-258">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="035a8-258">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="035a8-259">симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-259">simSetupScreenDisabled</span></span>|<span data-ttu-id="035a8-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-260">Boolean</span></span>|<span data-ttu-id="035a8-261">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="035a8-261">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="035a8-262">софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-262">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="035a8-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-263">Boolean</span></span>|<span data-ttu-id="035a8-264">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="035a8-264">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="035a8-265">ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-265">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="035a8-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-266">Boolean</span></span>|<span data-ttu-id="035a8-267">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="035a8-267">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="035a8-268">аппеаранцескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-268">appearanceScreenDisabled</span></span>|<span data-ttu-id="035a8-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-269">Boolean</span></span>|<span data-ttu-id="035a8-270">Указывает, отключен ли экран Апперанце</span><span class="sxs-lookup"><span data-stu-id="035a8-270">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="035a8-271">експресслангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-271">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="035a8-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-272">Boolean</span></span>|<span data-ttu-id="035a8-273">Указывает, отключен ли экран Express Language</span><span class="sxs-lookup"><span data-stu-id="035a8-273">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="035a8-274">преферредлангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-274">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="035a8-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-275">Boolean</span></span>|<span data-ttu-id="035a8-276">Указывает, отключен ли предпочтительный экран языка</span><span class="sxs-lookup"><span data-stu-id="035a8-276">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="035a8-277">девицетодевицемигратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-277">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="035a8-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-278">Boolean</span></span>|<span data-ttu-id="035a8-279">Указывает, отключена ли миграция устройств для устройств</span><span class="sxs-lookup"><span data-stu-id="035a8-279">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="035a8-280">велкомескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="035a8-280">welcomeScreenDisabled</span></span>|<span data-ttu-id="035a8-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="035a8-281">Boolean</span></span>|<span data-ttu-id="035a8-282">Указывает, отключен ли экран Векломе</span><span class="sxs-lookup"><span data-stu-id="035a8-282">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="035a8-283">Ответ</span><span class="sxs-lookup"><span data-stu-id="035a8-283">Response</span></span>
<span data-ttu-id="035a8-284">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="035a8-284">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="035a8-285">Пример</span><span class="sxs-lookup"><span data-stu-id="035a8-285">Example</span></span>

### <a name="request"></a><span data-ttu-id="035a8-286">Запрос</span><span class="sxs-lookup"><span data-stu-id="035a8-286">Request</span></span>
<span data-ttu-id="035a8-287">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="035a8-287">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 2024

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
  "welcomeScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="035a8-288">Отклик</span><span class="sxs-lookup"><span data-stu-id="035a8-288">Response</span></span>
<span data-ttu-id="035a8-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="035a8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2073

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
  "welcomeScreenDisabled": true
}
```





