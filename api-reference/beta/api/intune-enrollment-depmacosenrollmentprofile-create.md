---
title: Создание Депмакосенроллментпрофиле
description: Создание нового объекта Депмакосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53130ff00a97966a1498b89879c25b2f18d701fb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424731"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="a951e-103">Создание Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a951e-103">Create depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="a951e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a951e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a951e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a951e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a951e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a951e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a951e-107">Создание нового объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a951e-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a951e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a951e-108">Prerequisites</span></span>
<span data-ttu-id="a951e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a951e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a951e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a951e-111">Permission type</span></span>|<span data-ttu-id="a951e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a951e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a951e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a951e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a951e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a951e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a951e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a951e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a951e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a951e-116">Not supported.</span></span>|
|<span data-ttu-id="a951e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a951e-117">Application</span></span>|<span data-ttu-id="a951e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a951e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a951e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a951e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a951e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a951e-120">Request headers</span></span>
|<span data-ttu-id="a951e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a951e-121">Header</span></span>|<span data-ttu-id="a951e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a951e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a951e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a951e-123">Authorization</span></span>|<span data-ttu-id="a951e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a951e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a951e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a951e-125">Accept</span></span>|<span data-ttu-id="a951e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a951e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a951e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a951e-127">Request body</span></span>
<span data-ttu-id="a951e-128">В тексте запроса добавьте представление объекта Депмакосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a951e-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="a951e-129">В следующей таблице приведены свойства, необходимые при создании Депмакосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="a951e-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="a951e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a951e-130">Property</span></span>|<span data-ttu-id="a951e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a951e-131">Type</span></span>|<span data-ttu-id="a951e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a951e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a951e-133">id</span><span class="sxs-lookup"><span data-stu-id="a951e-133">id</span></span>|<span data-ttu-id="a951e-134">String</span><span class="sxs-lookup"><span data-stu-id="a951e-134">String</span></span>|<span data-ttu-id="a951e-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a951e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a951e-136">displayName</span></span>|<span data-ttu-id="a951e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a951e-137">String</span></span>|<span data-ttu-id="a951e-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a951e-139">description</span><span class="sxs-lookup"><span data-stu-id="a951e-139">description</span></span>|<span data-ttu-id="a951e-140">String</span><span class="sxs-lookup"><span data-stu-id="a951e-140">String</span></span>|<span data-ttu-id="a951e-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a951e-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="a951e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="a951e-143">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-143">Boolean</span></span>|<span data-ttu-id="a951e-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a951e-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="a951e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="a951e-146">String</span><span class="sxs-lookup"><span data-stu-id="a951e-146">String</span></span>|<span data-ttu-id="a951e-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a951e-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="a951e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="a951e-149">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-149">Boolean</span></span>|<span data-ttu-id="a951e-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="a951e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="a951e-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a951e-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="a951e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="a951e-153">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-153">Boolean</span></span>|<span data-ttu-id="a951e-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a951e-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="a951e-155">isDefault</span></span>|<span data-ttu-id="a951e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a951e-156">Boolean</span></span>|<span data-ttu-id="a951e-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-158">supervisedModeEnabled</span></span>|<span data-ttu-id="a951e-159">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-159">Boolean</span></span>|<span data-ttu-id="a951e-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="a951e-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="a951e-161">Дополнительную https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="a951e-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="a951e-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="a951e-163">supportDepartment</span></span>|<span data-ttu-id="a951e-164">String</span><span class="sxs-lookup"><span data-stu-id="a951e-164">String</span></span>|<span data-ttu-id="a951e-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-166">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-166">passCodeDisabled</span></span>|<span data-ttu-id="a951e-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-167">Boolean</span></span>|<span data-ttu-id="a951e-168">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-169">Обязательный</span><span class="sxs-lookup"><span data-stu-id="a951e-169">isMandatory</span></span>|<span data-ttu-id="a951e-170">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-170">Boolean</span></span>|<span data-ttu-id="a951e-171">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-172">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-172">locationDisabled</span></span>|<span data-ttu-id="a951e-173">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-173">Boolean</span></span>|<span data-ttu-id="a951e-174">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-175">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="a951e-175">supportPhoneNumber</span></span>|<span data-ttu-id="a951e-176">String</span><span class="sxs-lookup"><span data-stu-id="a951e-176">String</span></span>|<span data-ttu-id="a951e-177">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-178">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-178">profileRemovalDisabled</span></span>|<span data-ttu-id="a951e-179">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-179">Boolean</span></span>|<span data-ttu-id="a951e-180">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-181">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="a951e-181">restoreBlocked</span></span>|<span data-ttu-id="a951e-182">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-182">Boolean</span></span>|<span data-ttu-id="a951e-183">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-184">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-184">appleIdDisabled</span></span>|<span data-ttu-id="a951e-185">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-185">Boolean</span></span>|<span data-ttu-id="a951e-186">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-187">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="a951e-188">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-188">Boolean</span></span>|<span data-ttu-id="a951e-189">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-190">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-190">touchIdDisabled</span></span>|<span data-ttu-id="a951e-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-191">Boolean</span></span>|<span data-ttu-id="a951e-192">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-193">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-193">applePayDisabled</span></span>|<span data-ttu-id="a951e-194">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-194">Boolean</span></span>|<span data-ttu-id="a951e-195">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-196">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-196">zoomDisabled</span></span>|<span data-ttu-id="a951e-197">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-197">Boolean</span></span>|<span data-ttu-id="a951e-198">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-199">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-199">siriDisabled</span></span>|<span data-ttu-id="a951e-200">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-200">Boolean</span></span>|<span data-ttu-id="a951e-201">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-202">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-202">diagnosticsDisabled</span></span>|<span data-ttu-id="a951e-203">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-203">Boolean</span></span>|<span data-ttu-id="a951e-204">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-205">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="a951e-206">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-206">Boolean</span></span>|<span data-ttu-id="a951e-207">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-208">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-208">privacyPaneDisabled</span></span>|<span data-ttu-id="a951e-209">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-209">Boolean</span></span>|<span data-ttu-id="a951e-210">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-211">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="a951e-212">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-212">Boolean</span></span>|<span data-ttu-id="a951e-213">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-214">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="a951e-214">deviceNameTemplate</span></span>|<span data-ttu-id="a951e-215">String</span><span class="sxs-lookup"><span data-stu-id="a951e-215">String</span></span>|<span data-ttu-id="a951e-216">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="a951e-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="a951e-217">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-218">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="a951e-218">configurationWebUrl</span></span>|<span data-ttu-id="a951e-219">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-219">Boolean</span></span>|<span data-ttu-id="a951e-220">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a951e-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a951e-221">регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-221">registrationDisabled</span></span>|<span data-ttu-id="a951e-222">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-222">Boolean</span></span>|<span data-ttu-id="a951e-223">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="a951e-223">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="a951e-224">филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-224">fileVaultDisabled</span></span>|<span data-ttu-id="a951e-225">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-225">Boolean</span></span>|<span data-ttu-id="a951e-226">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="a951e-226">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="a951e-227">иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-227">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="a951e-228">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-228">Boolean</span></span>|<span data-ttu-id="a951e-229">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="a951e-229">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="a951e-230">иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="a951e-231">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-231">Boolean</span></span>|<span data-ttu-id="a951e-232">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="a951e-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="a951e-233">чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a951e-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="a951e-234">Логическое</span><span class="sxs-lookup"><span data-stu-id="a951e-234">Boolean</span></span>|<span data-ttu-id="a951e-235">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="a951e-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="a951e-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="a951e-236">Response</span></span>
<span data-ttu-id="a951e-237">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a951e-237">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a951e-238">Пример</span><span class="sxs-lookup"><span data-stu-id="a951e-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="a951e-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="a951e-239">Request</span></span>
<span data-ttu-id="a951e-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a951e-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1260

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="a951e-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="a951e-241">Response</span></span>
<span data-ttu-id="a951e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a951e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1309

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```



