---
title: Обновление Депиосенроллментпрофиле
description: Обновление свойств объекта Депиосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b611d734919679724d194649f66f549b499bc9c1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424770"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="d6c46-103">Обновление Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="d6c46-103">Update depIOSEnrollmentProfile</span></span>

<span data-ttu-id="d6c46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6c46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6c46-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6c46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6c46-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6c46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6c46-107">Обновление свойств объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d6c46-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6c46-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6c46-108">Prerequisites</span></span>
<span data-ttu-id="d6c46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6c46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6c46-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6c46-111">Permission type</span></span>|<span data-ttu-id="d6c46-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6c46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6c46-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6c46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6c46-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c46-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d6c46-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6c46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6c46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6c46-116">Not supported.</span></span>|
|<span data-ttu-id="d6c46-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6c46-117">Application</span></span>|<span data-ttu-id="d6c46-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c46-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6c46-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6c46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="d6c46-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6c46-120">Request headers</span></span>
|<span data-ttu-id="d6c46-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6c46-121">Header</span></span>|<span data-ttu-id="d6c46-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6c46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6c46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6c46-123">Authorization</span></span>|<span data-ttu-id="d6c46-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6c46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6c46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6c46-125">Accept</span></span>|<span data-ttu-id="d6c46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6c46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6c46-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6c46-127">Request body</span></span>
<span data-ttu-id="d6c46-128">В тексте запроса добавьте представление объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6c46-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d6c46-129">В следующей таблице приведены свойства, необходимые при создании [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d6c46-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="d6c46-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6c46-130">Property</span></span>|<span data-ttu-id="d6c46-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6c46-131">Type</span></span>|<span data-ttu-id="d6c46-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6c46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c46-133">id</span><span class="sxs-lookup"><span data-stu-id="d6c46-133">id</span></span>|<span data-ttu-id="d6c46-134">String</span><span class="sxs-lookup"><span data-stu-id="d6c46-134">String</span></span>|<span data-ttu-id="d6c46-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d6c46-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d6c46-136">displayName</span></span>|<span data-ttu-id="d6c46-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d6c46-137">String</span></span>|<span data-ttu-id="d6c46-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d6c46-139">description</span><span class="sxs-lookup"><span data-stu-id="d6c46-139">description</span></span>|<span data-ttu-id="d6c46-140">String</span><span class="sxs-lookup"><span data-stu-id="d6c46-140">String</span></span>|<span data-ttu-id="d6c46-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d6c46-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="d6c46-142">requiresUserAuthentication</span></span>|<span data-ttu-id="d6c46-143">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-143">Boolean</span></span>|<span data-ttu-id="d6c46-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d6c46-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="d6c46-145">configurationEndpointUrl</span></span>|<span data-ttu-id="d6c46-146">String</span><span class="sxs-lookup"><span data-stu-id="d6c46-146">String</span></span>|<span data-ttu-id="d6c46-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d6c46-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d6c46-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d6c46-149">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-149">Boolean</span></span>|<span data-ttu-id="d6c46-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="d6c46-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d6c46-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d6c46-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="d6c46-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d6c46-153">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-153">Boolean</span></span>|<span data-ttu-id="d6c46-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d6c46-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="d6c46-155">isDefault</span></span>|<span data-ttu-id="d6c46-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6c46-156">Boolean</span></span>|<span data-ttu-id="d6c46-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-158">supervisedModeEnabled</span></span>|<span data-ttu-id="d6c46-159">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-159">Boolean</span></span>|<span data-ttu-id="d6c46-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="d6c46-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d6c46-161">Дополнительную https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="d6c46-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="d6c46-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="d6c46-163">supportDepartment</span></span>|<span data-ttu-id="d6c46-164">String</span><span class="sxs-lookup"><span data-stu-id="d6c46-164">String</span></span>|<span data-ttu-id="d6c46-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-166">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-166">passCodeDisabled</span></span>|<span data-ttu-id="d6c46-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-167">Boolean</span></span>|<span data-ttu-id="d6c46-168">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-169">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d6c46-169">isMandatory</span></span>|<span data-ttu-id="d6c46-170">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-170">Boolean</span></span>|<span data-ttu-id="d6c46-171">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-172">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-172">locationDisabled</span></span>|<span data-ttu-id="d6c46-173">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-173">Boolean</span></span>|<span data-ttu-id="d6c46-174">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-175">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="d6c46-175">supportPhoneNumber</span></span>|<span data-ttu-id="d6c46-176">String</span><span class="sxs-lookup"><span data-stu-id="d6c46-176">String</span></span>|<span data-ttu-id="d6c46-177">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-178">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-178">profileRemovalDisabled</span></span>|<span data-ttu-id="d6c46-179">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-179">Boolean</span></span>|<span data-ttu-id="d6c46-180">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-181">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="d6c46-181">restoreBlocked</span></span>|<span data-ttu-id="d6c46-182">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-182">Boolean</span></span>|<span data-ttu-id="d6c46-183">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-184">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-184">appleIdDisabled</span></span>|<span data-ttu-id="d6c46-185">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-185">Boolean</span></span>|<span data-ttu-id="d6c46-186">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-187">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d6c46-188">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-188">Boolean</span></span>|<span data-ttu-id="d6c46-189">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-190">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-190">touchIdDisabled</span></span>|<span data-ttu-id="d6c46-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-191">Boolean</span></span>|<span data-ttu-id="d6c46-192">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-193">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-193">applePayDisabled</span></span>|<span data-ttu-id="d6c46-194">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-194">Boolean</span></span>|<span data-ttu-id="d6c46-195">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-196">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-196">zoomDisabled</span></span>|<span data-ttu-id="d6c46-197">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-197">Boolean</span></span>|<span data-ttu-id="d6c46-198">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-199">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-199">siriDisabled</span></span>|<span data-ttu-id="d6c46-200">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-200">Boolean</span></span>|<span data-ttu-id="d6c46-201">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-202">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-202">diagnosticsDisabled</span></span>|<span data-ttu-id="d6c46-203">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-203">Boolean</span></span>|<span data-ttu-id="d6c46-204">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-205">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="d6c46-206">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-206">Boolean</span></span>|<span data-ttu-id="d6c46-207">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-208">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-208">privacyPaneDisabled</span></span>|<span data-ttu-id="d6c46-209">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-209">Boolean</span></span>|<span data-ttu-id="d6c46-210">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-211">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="d6c46-212">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-212">Boolean</span></span>|<span data-ttu-id="d6c46-213">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-214">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="d6c46-214">deviceNameTemplate</span></span>|<span data-ttu-id="d6c46-215">String</span><span class="sxs-lookup"><span data-stu-id="d6c46-215">String</span></span>|<span data-ttu-id="d6c46-216">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="d6c46-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="d6c46-217">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-218">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="d6c46-218">configurationWebUrl</span></span>|<span data-ttu-id="d6c46-219">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-219">Boolean</span></span>|<span data-ttu-id="d6c46-220">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d6c46-221">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d6c46-221">iTunesPairingMode</span></span>|<span data-ttu-id="d6c46-222">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="d6c46-222">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="d6c46-223">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="d6c46-223">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="d6c46-224">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="d6c46-224">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="d6c46-225">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="d6c46-225">managementCertificates</span></span>|<span data-ttu-id="d6c46-226">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="d6c46-226">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="d6c46-227">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="d6c46-227">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="d6c46-228">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-228">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="d6c46-229">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-229">Boolean</span></span>|<span data-ttu-id="d6c46-230">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="d6c46-230">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="d6c46-231">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="d6c46-231">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="d6c46-232">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-232">Boolean</span></span>|<span data-ttu-id="d6c46-233">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="d6c46-233">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="d6c46-234">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="d6c46-234">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="d6c46-235">Int32</span><span class="sxs-lookup"><span data-stu-id="d6c46-235">Int32</span></span>|<span data-ttu-id="d6c46-236">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="d6c46-236">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="d6c46-237">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="d6c46-237">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="d6c46-238">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="d6c46-238">enableSharedIPad</span></span>|<span data-ttu-id="d6c46-239">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-239">Boolean</span></span>|<span data-ttu-id="d6c46-240">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="d6c46-240">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="d6c46-241">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="d6c46-241">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="d6c46-242">компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="d6c46-242">companyPortalVppTokenId</span></span>|<span data-ttu-id="d6c46-243">String</span><span class="sxs-lookup"><span data-stu-id="d6c46-243">String</span></span>|<span data-ttu-id="d6c46-244">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="d6c46-244">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="d6c46-245">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="d6c46-245">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="d6c46-246">енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="d6c46-246">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="d6c46-247">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-247">Boolean</span></span>|<span data-ttu-id="d6c46-248">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="d6c46-248">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="d6c46-249">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="d6c46-249">Default is false.</span></span> <span data-ttu-id="d6c46-250">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="d6c46-250">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="d6c46-251">хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-251">homeButtonScreenDisabled</span></span>|<span data-ttu-id="d6c46-252">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-252">Boolean</span></span>|<span data-ttu-id="d6c46-253">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="d6c46-253">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="d6c46-254">имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-254">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="d6c46-255">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-255">Boolean</span></span>|<span data-ttu-id="d6c46-256">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="d6c46-256">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="d6c46-257">онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-257">onBoardingScreenDisabled</span></span>|<span data-ttu-id="d6c46-258">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-258">Boolean</span></span>|<span data-ttu-id="d6c46-259">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="d6c46-259">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="d6c46-260">симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-260">simSetupScreenDisabled</span></span>|<span data-ttu-id="d6c46-261">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-261">Boolean</span></span>|<span data-ttu-id="d6c46-262">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="d6c46-262">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="d6c46-263">софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-263">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="d6c46-264">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-264">Boolean</span></span>|<span data-ttu-id="d6c46-265">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="d6c46-265">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="d6c46-266">ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-266">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="d6c46-267">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-267">Boolean</span></span>|<span data-ttu-id="d6c46-268">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="d6c46-268">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="d6c46-269">аппеаранцескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-269">appearanceScreenDisabled</span></span>|<span data-ttu-id="d6c46-270">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-270">Boolean</span></span>|<span data-ttu-id="d6c46-271">Указывает, отключен ли экран Апперанце</span><span class="sxs-lookup"><span data-stu-id="d6c46-271">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="d6c46-272">експресслангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-272">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="d6c46-273">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-273">Boolean</span></span>|<span data-ttu-id="d6c46-274">Указывает, отключен ли экран Express Language</span><span class="sxs-lookup"><span data-stu-id="d6c46-274">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="d6c46-275">преферредлангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-275">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="d6c46-276">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-276">Boolean</span></span>|<span data-ttu-id="d6c46-277">Указывает, отключен ли предпочтительный экран языка</span><span class="sxs-lookup"><span data-stu-id="d6c46-277">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="d6c46-278">девицетодевицемигратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-278">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="d6c46-279">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-279">Boolean</span></span>|<span data-ttu-id="d6c46-280">Указывает, отключена ли миграция устройств для устройств</span><span class="sxs-lookup"><span data-stu-id="d6c46-280">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="d6c46-281">велкомескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d6c46-281">welcomeScreenDisabled</span></span>|<span data-ttu-id="d6c46-282">Логическое</span><span class="sxs-lookup"><span data-stu-id="d6c46-282">Boolean</span></span>|<span data-ttu-id="d6c46-283">Указывает, отключен ли экран Векломе</span><span class="sxs-lookup"><span data-stu-id="d6c46-283">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="d6c46-284">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6c46-284">Response</span></span>
<span data-ttu-id="d6c46-285">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6c46-285">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6c46-286">Пример</span><span class="sxs-lookup"><span data-stu-id="d6c46-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6c46-287">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6c46-287">Request</span></span>
<span data-ttu-id="d6c46-288">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6c46-288">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d6c46-289">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6c46-289">Response</span></span>
<span data-ttu-id="d6c46-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6c46-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



