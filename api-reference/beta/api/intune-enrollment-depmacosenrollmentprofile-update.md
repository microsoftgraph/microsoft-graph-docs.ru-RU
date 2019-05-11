---
title: Обновление Депмакосенроллментпрофиле
description: Обновление свойств объекта Депмакосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 238676c0c1ea2019c6f505b55fb5db398d248d2b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908772"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="0a762-103">Обновление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0a762-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="0a762-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a762-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a762-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a762-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a762-106">Обновление свойств объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0a762-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a762-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a762-107">Prerequisites</span></span>
<span data-ttu-id="0a762-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a762-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a762-110">Permission type</span></span>|<span data-ttu-id="0a762-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a762-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a762-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a762-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a762-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a762-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a762-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a762-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a762-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a762-115">Not supported.</span></span>|
|<span data-ttu-id="0a762-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a762-116">Application</span></span>|<span data-ttu-id="0a762-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a762-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a762-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a762-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="0a762-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a762-119">Request headers</span></span>
|<span data-ttu-id="0a762-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a762-120">Header</span></span>|<span data-ttu-id="0a762-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0a762-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a762-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a762-122">Authorization</span></span>|<span data-ttu-id="0a762-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a762-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a762-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0a762-124">Accept</span></span>|<span data-ttu-id="0a762-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a762-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a762-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a762-126">Request body</span></span>
<span data-ttu-id="0a762-127">В тексте запроса добавьте представление объекта [Депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a762-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="0a762-128">В следующей таблице приведены свойства, необходимые при создании [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0a762-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="0a762-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a762-129">Property</span></span>|<span data-ttu-id="0a762-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0a762-130">Type</span></span>|<span data-ttu-id="0a762-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0a762-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a762-132">id</span><span class="sxs-lookup"><span data-stu-id="0a762-132">id</span></span>|<span data-ttu-id="0a762-133">String</span><span class="sxs-lookup"><span data-stu-id="0a762-133">String</span></span>|<span data-ttu-id="0a762-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0a762-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0a762-135">displayName</span></span>|<span data-ttu-id="0a762-136">Строка</span><span class="sxs-lookup"><span data-stu-id="0a762-136">String</span></span>|<span data-ttu-id="0a762-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0a762-138">description</span><span class="sxs-lookup"><span data-stu-id="0a762-138">description</span></span>|<span data-ttu-id="0a762-139">String</span><span class="sxs-lookup"><span data-stu-id="0a762-139">String</span></span>|<span data-ttu-id="0a762-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0a762-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="0a762-141">requiresUserAuthentication</span></span>|<span data-ttu-id="0a762-142">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-142">Boolean</span></span>|<span data-ttu-id="0a762-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0a762-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="0a762-144">configurationEndpointUrl</span></span>|<span data-ttu-id="0a762-145">Строка</span><span class="sxs-lookup"><span data-stu-id="0a762-145">String</span></span>|<span data-ttu-id="0a762-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0a762-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="0a762-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="0a762-148">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-148">Boolean</span></span>|<span data-ttu-id="0a762-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="0a762-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="0a762-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0a762-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="0a762-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="0a762-152">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-152">Boolean</span></span>|<span data-ttu-id="0a762-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0a762-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="0a762-154">isDefault</span></span>|<span data-ttu-id="0a762-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a762-155">Boolean</span></span>|<span data-ttu-id="0a762-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-157">supervisedModeEnabled</span></span>|<span data-ttu-id="0a762-158">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-158">Boolean</span></span>|<span data-ttu-id="0a762-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="0a762-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="0a762-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="0a762-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="0a762-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-162">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="0a762-162">supportDepartment</span></span>|<span data-ttu-id="0a762-163">Строка</span><span class="sxs-lookup"><span data-stu-id="0a762-163">String</span></span>|<span data-ttu-id="0a762-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-165">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-165">passCodeDisabled</span></span>|<span data-ttu-id="0a762-166">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-166">Boolean</span></span>|<span data-ttu-id="0a762-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0a762-168">isMandatory</span></span>|<span data-ttu-id="0a762-169">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-169">Boolean</span></span>|<span data-ttu-id="0a762-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-171">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-171">locationDisabled</span></span>|<span data-ttu-id="0a762-172">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-172">Boolean</span></span>|<span data-ttu-id="0a762-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-174">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="0a762-174">supportPhoneNumber</span></span>|<span data-ttu-id="0a762-175">Строка</span><span class="sxs-lookup"><span data-stu-id="0a762-175">String</span></span>|<span data-ttu-id="0a762-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-177">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-177">profileRemovalDisabled</span></span>|<span data-ttu-id="0a762-178">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-178">Boolean</span></span>|<span data-ttu-id="0a762-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-180">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="0a762-180">restoreBlocked</span></span>|<span data-ttu-id="0a762-181">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-181">Boolean</span></span>|<span data-ttu-id="0a762-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-183">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-183">appleIdDisabled</span></span>|<span data-ttu-id="0a762-184">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-184">Boolean</span></span>|<span data-ttu-id="0a762-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-186">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="0a762-187">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-187">Boolean</span></span>|<span data-ttu-id="0a762-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-189">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-189">touchIdDisabled</span></span>|<span data-ttu-id="0a762-190">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-190">Boolean</span></span>|<span data-ttu-id="0a762-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-192">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-192">applePayDisabled</span></span>|<span data-ttu-id="0a762-193">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-193">Boolean</span></span>|<span data-ttu-id="0a762-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-195">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-195">zoomDisabled</span></span>|<span data-ttu-id="0a762-196">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-196">Boolean</span></span>|<span data-ttu-id="0a762-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-198">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-198">siriDisabled</span></span>|<span data-ttu-id="0a762-199">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-199">Boolean</span></span>|<span data-ttu-id="0a762-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-201">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-201">diagnosticsDisabled</span></span>|<span data-ttu-id="0a762-202">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-202">Boolean</span></span>|<span data-ttu-id="0a762-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-204">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="0a762-205">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-205">Boolean</span></span>|<span data-ttu-id="0a762-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-207">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-207">privacyPaneDisabled</span></span>|<span data-ttu-id="0a762-208">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-208">Boolean</span></span>|<span data-ttu-id="0a762-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-210">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="0a762-210">deviceNameTemplate</span></span>|<span data-ttu-id="0a762-211">Строка</span><span class="sxs-lookup"><span data-stu-id="0a762-211">String</span></span>|<span data-ttu-id="0a762-212">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="0a762-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="0a762-213">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0a762-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0a762-214">Регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-214">registrationDisabled</span></span>|<span data-ttu-id="0a762-215">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-215">Boolean</span></span>|<span data-ttu-id="0a762-216">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="0a762-216">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="0a762-217">Филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-217">fileVaultDisabled</span></span>|<span data-ttu-id="0a762-218">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-218">Boolean</span></span>|<span data-ttu-id="0a762-219">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="0a762-219">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="0a762-220">Иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-220">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="0a762-221">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-221">Boolean</span></span>|<span data-ttu-id="0a762-222">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="0a762-222">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="0a762-223">Иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-223">iCloudStorageDisabled</span></span>|<span data-ttu-id="0a762-224">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-224">Boolean</span></span>|<span data-ttu-id="0a762-225">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="0a762-225">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="0a762-226">Чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="0a762-226">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="0a762-227">Логический</span><span class="sxs-lookup"><span data-stu-id="0a762-227">Boolean</span></span>|<span data-ttu-id="0a762-228">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="0a762-228">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="0a762-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a762-229">Response</span></span>
<span data-ttu-id="0a762-230">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a762-230">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a762-231">Пример</span><span class="sxs-lookup"><span data-stu-id="0a762-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a762-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a762-232">Request</span></span>
<span data-ttu-id="0a762-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a762-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1191

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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="0a762-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a762-234">Response</span></span>
<span data-ttu-id="0a762-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a762-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1240

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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```




