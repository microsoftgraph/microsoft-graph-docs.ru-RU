---
title: Обновление Депмакосенроллментпрофиле
description: Обновление свойств объекта Депмакосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d0018e0451a87d0dc2152c9dfd5645dc533ecdf6
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536022"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="55eb0-103">Обновление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="55eb0-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="55eb0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55eb0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55eb0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55eb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55eb0-106">Обновление свойств объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="55eb0-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55eb0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55eb0-107">Prerequisites</span></span>
<span data-ttu-id="55eb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55eb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55eb0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55eb0-110">Permission type</span></span>|<span data-ttu-id="55eb0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55eb0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55eb0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55eb0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55eb0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55eb0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="55eb0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55eb0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55eb0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55eb0-115">Not supported.</span></span>|
|<span data-ttu-id="55eb0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="55eb0-116">Application</span></span>|<span data-ttu-id="55eb0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55eb0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55eb0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55eb0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="55eb0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55eb0-119">Request headers</span></span>
|<span data-ttu-id="55eb0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55eb0-120">Header</span></span>|<span data-ttu-id="55eb0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="55eb0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55eb0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55eb0-122">Authorization</span></span>|<span data-ttu-id="55eb0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55eb0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55eb0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="55eb0-124">Accept</span></span>|<span data-ttu-id="55eb0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55eb0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55eb0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55eb0-126">Request body</span></span>
<span data-ttu-id="55eb0-127">В тексте запроса добавьте представление объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55eb0-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="55eb0-128">В следующей таблице приведены свойства, необходимые при создании [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="55eb0-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="55eb0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="55eb0-129">Property</span></span>|<span data-ttu-id="55eb0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="55eb0-130">Type</span></span>|<span data-ttu-id="55eb0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="55eb0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55eb0-132">id</span><span class="sxs-lookup"><span data-stu-id="55eb0-132">id</span></span>|<span data-ttu-id="55eb0-133">String</span><span class="sxs-lookup"><span data-stu-id="55eb0-133">String</span></span>|<span data-ttu-id="55eb0-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55eb0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="55eb0-135">displayName</span></span>|<span data-ttu-id="55eb0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="55eb0-136">String</span></span>|<span data-ttu-id="55eb0-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55eb0-138">description</span><span class="sxs-lookup"><span data-stu-id="55eb0-138">description</span></span>|<span data-ttu-id="55eb0-139">String</span><span class="sxs-lookup"><span data-stu-id="55eb0-139">String</span></span>|<span data-ttu-id="55eb0-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55eb0-141">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="55eb0-141">requiresUserAuthentication</span></span>|<span data-ttu-id="55eb0-142">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-142">Boolean</span></span>|<span data-ttu-id="55eb0-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55eb0-144">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="55eb0-144">configurationEndpointUrl</span></span>|<span data-ttu-id="55eb0-145">String</span><span class="sxs-lookup"><span data-stu-id="55eb0-145">String</span></span>|<span data-ttu-id="55eb0-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55eb0-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="55eb0-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="55eb0-148">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-148">Boolean</span></span>|<span data-ttu-id="55eb0-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="55eb0-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="55eb0-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55eb0-151">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="55eb0-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="55eb0-152">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-152">Boolean</span></span>|<span data-ttu-id="55eb0-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55eb0-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="55eb0-154">isDefault</span></span>|<span data-ttu-id="55eb0-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb0-155">Boolean</span></span>|<span data-ttu-id="55eb0-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-157">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-157">supervisedModeEnabled</span></span>|<span data-ttu-id="55eb0-158">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-158">Boolean</span></span>|<span data-ttu-id="55eb0-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="55eb0-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="55eb0-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="55eb0-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="55eb0-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-162">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="55eb0-162">supportDepartment</span></span>|<span data-ttu-id="55eb0-163">String</span><span class="sxs-lookup"><span data-stu-id="55eb0-163">String</span></span>|<span data-ttu-id="55eb0-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-165">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-165">passCodeDisabled</span></span>|<span data-ttu-id="55eb0-166">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-166">Boolean</span></span>|<span data-ttu-id="55eb0-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="55eb0-168">isMandatory</span></span>|<span data-ttu-id="55eb0-169">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-169">Boolean</span></span>|<span data-ttu-id="55eb0-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-171">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-171">locationDisabled</span></span>|<span data-ttu-id="55eb0-172">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-172">Boolean</span></span>|<span data-ttu-id="55eb0-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-174">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="55eb0-174">supportPhoneNumber</span></span>|<span data-ttu-id="55eb0-175">String</span><span class="sxs-lookup"><span data-stu-id="55eb0-175">String</span></span>|<span data-ttu-id="55eb0-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-177">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-177">profileRemovalDisabled</span></span>|<span data-ttu-id="55eb0-178">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-178">Boolean</span></span>|<span data-ttu-id="55eb0-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-180">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="55eb0-180">restoreBlocked</span></span>|<span data-ttu-id="55eb0-181">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-181">Boolean</span></span>|<span data-ttu-id="55eb0-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-183">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-183">appleIdDisabled</span></span>|<span data-ttu-id="55eb0-184">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-184">Boolean</span></span>|<span data-ttu-id="55eb0-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-186">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="55eb0-187">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-187">Boolean</span></span>|<span data-ttu-id="55eb0-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-189">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-189">touchIdDisabled</span></span>|<span data-ttu-id="55eb0-190">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-190">Boolean</span></span>|<span data-ttu-id="55eb0-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-192">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-192">applePayDisabled</span></span>|<span data-ttu-id="55eb0-193">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-193">Boolean</span></span>|<span data-ttu-id="55eb0-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-195">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-195">zoomDisabled</span></span>|<span data-ttu-id="55eb0-196">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-196">Boolean</span></span>|<span data-ttu-id="55eb0-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-198">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-198">siriDisabled</span></span>|<span data-ttu-id="55eb0-199">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-199">Boolean</span></span>|<span data-ttu-id="55eb0-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-201">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-201">diagnosticsDisabled</span></span>|<span data-ttu-id="55eb0-202">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-202">Boolean</span></span>|<span data-ttu-id="55eb0-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-204">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="55eb0-205">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-205">Boolean</span></span>|<span data-ttu-id="55eb0-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-207">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-207">privacyPaneDisabled</span></span>|<span data-ttu-id="55eb0-208">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-208">Boolean</span></span>|<span data-ttu-id="55eb0-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-210">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="55eb0-211">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-211">Boolean</span></span>|<span data-ttu-id="55eb0-212">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-213">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="55eb0-213">deviceNameTemplate</span></span>|<span data-ttu-id="55eb0-214">String</span><span class="sxs-lookup"><span data-stu-id="55eb0-214">String</span></span>|<span data-ttu-id="55eb0-215">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="55eb0-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="55eb0-216">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-217">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="55eb0-217">configurationWebUrl</span></span>|<span data-ttu-id="55eb0-218">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-218">Boolean</span></span>|<span data-ttu-id="55eb0-219">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55eb0-219">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55eb0-220">регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-220">registrationDisabled</span></span>|<span data-ttu-id="55eb0-221">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-221">Boolean</span></span>|<span data-ttu-id="55eb0-222">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="55eb0-222">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="55eb0-223">филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-223">fileVaultDisabled</span></span>|<span data-ttu-id="55eb0-224">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-224">Boolean</span></span>|<span data-ttu-id="55eb0-225">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="55eb0-225">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="55eb0-226">иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-226">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="55eb0-227">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-227">Boolean</span></span>|<span data-ttu-id="55eb0-228">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="55eb0-228">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="55eb0-229">иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-229">iCloudStorageDisabled</span></span>|<span data-ttu-id="55eb0-230">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-230">Boolean</span></span>|<span data-ttu-id="55eb0-231">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="55eb0-231">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="55eb0-232">чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="55eb0-232">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="55eb0-233">Логический</span><span class="sxs-lookup"><span data-stu-id="55eb0-233">Boolean</span></span>|<span data-ttu-id="55eb0-234">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="55eb0-234">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="55eb0-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="55eb0-235">Response</span></span>
<span data-ttu-id="55eb0-236">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55eb0-236">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55eb0-237">Пример</span><span class="sxs-lookup"><span data-stu-id="55eb0-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="55eb0-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="55eb0-238">Request</span></span>
<span data-ttu-id="55eb0-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55eb0-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="55eb0-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="55eb0-240">Response</span></span>
<span data-ttu-id="55eb0-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55eb0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






