---
title: Обновление Депиосенроллментпрофиле
description: Обновление свойств объекта Депиосенроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89ce85e09ee9ad59c19c67401238e2f0f950eaba
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167734"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="f4d78-103">Обновление Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="f4d78-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="f4d78-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4d78-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4d78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4d78-106">Обновление свойств объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f4d78-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4d78-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4d78-107">Prerequisites</span></span>
<span data-ttu-id="f4d78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4d78-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d78-110">Permission type</span></span>|<span data-ttu-id="f4d78-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4d78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4d78-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4d78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4d78-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d78-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4d78-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4d78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4d78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d78-115">Not supported.</span></span>|
|<span data-ttu-id="f4d78-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4d78-116">Application</span></span>|<span data-ttu-id="f4d78-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4d78-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4d78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="f4d78-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4d78-119">Request headers</span></span>
|<span data-ttu-id="f4d78-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4d78-120">Header</span></span>|<span data-ttu-id="f4d78-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4d78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4d78-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4d78-122">Authorization</span></span>|<span data-ttu-id="f4d78-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f4d78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4d78-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4d78-124">Accept</span></span>|<span data-ttu-id="f4d78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4d78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4d78-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4d78-126">Request body</span></span>
<span data-ttu-id="f4d78-127">В тексте запроса добавьте представление объекта [Депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4d78-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="f4d78-128">В следующей таблице приведены свойства, необходимые при создании [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f4d78-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="f4d78-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4d78-129">Property</span></span>|<span data-ttu-id="f4d78-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f4d78-130">Type</span></span>|<span data-ttu-id="f4d78-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f4d78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4d78-132">id</span><span class="sxs-lookup"><span data-stu-id="f4d78-132">id</span></span>|<span data-ttu-id="f4d78-133">String</span><span class="sxs-lookup"><span data-stu-id="f4d78-133">String</span></span>|<span data-ttu-id="f4d78-134">GUID объекта, наСледуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4d78-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f4d78-135">displayName</span></span>|<span data-ttu-id="f4d78-136">String</span><span class="sxs-lookup"><span data-stu-id="f4d78-136">String</span></span>|<span data-ttu-id="f4d78-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4d78-138">description</span><span class="sxs-lookup"><span data-stu-id="f4d78-138">description</span></span>|<span data-ttu-id="f4d78-139">String</span><span class="sxs-lookup"><span data-stu-id="f4d78-139">String</span></span>|<span data-ttu-id="f4d78-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4d78-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="f4d78-141">requiresUserAuthentication</span></span>|<span data-ttu-id="f4d78-142">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-142">Boolean</span></span>|<span data-ttu-id="f4d78-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4d78-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="f4d78-144">configurationEndpointUrl</span></span>|<span data-ttu-id="f4d78-145">String</span><span class="sxs-lookup"><span data-stu-id="f4d78-145">String</span></span>|<span data-ttu-id="f4d78-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4d78-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="f4d78-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f4d78-148">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-148">Boolean</span></span>|<span data-ttu-id="f4d78-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="f4d78-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f4d78-150">НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4d78-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="f4d78-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f4d78-152">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-152">Boolean</span></span>|<span data-ttu-id="f4d78-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наСледуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f4d78-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="f4d78-154">isDefault</span></span>|<span data-ttu-id="f4d78-155">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-155">Boolean</span></span>|<span data-ttu-id="f4d78-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-157">supervisedModeEnabled</span></span>|<span data-ttu-id="f4d78-158">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-158">Boolean</span></span>|<span data-ttu-id="f4d78-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="f4d78-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f4d78-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="f4d78-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="f4d78-161">НаСледуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-162">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="f4d78-162">supportDepartment</span></span>|<span data-ttu-id="f4d78-163">String</span><span class="sxs-lookup"><span data-stu-id="f4d78-163">String</span></span>|<span data-ttu-id="f4d78-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-165">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-165">passCodeDisabled</span></span>|<span data-ttu-id="f4d78-166">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-166">Boolean</span></span>|<span data-ttu-id="f4d78-167">Указывает, является ли область настройки секретного кода наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f4d78-168">isMandatory</span></span>|<span data-ttu-id="f4d78-169">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-169">Boolean</span></span>|<span data-ttu-id="f4d78-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-171">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-171">locationDisabled</span></span>|<span data-ttu-id="f4d78-172">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-172">Boolean</span></span>|<span data-ttu-id="f4d78-173">Указывает, является ли область настроек службы расположений наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-174">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="f4d78-174">supportPhoneNumber</span></span>|<span data-ttu-id="f4d78-175">String</span><span class="sxs-lookup"><span data-stu-id="f4d78-175">String</span></span>|<span data-ttu-id="f4d78-176">Номер телефона поддержки, наСледуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-177">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-177">profileRemovalDisabled</span></span>|<span data-ttu-id="f4d78-178">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-178">Boolean</span></span>|<span data-ttu-id="f4d78-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-180">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="f4d78-180">restoreBlocked</span></span>|<span data-ttu-id="f4d78-181">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-181">Boolean</span></span>|<span data-ttu-id="f4d78-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-183">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-183">appleIdDisabled</span></span>|<span data-ttu-id="f4d78-184">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-184">Boolean</span></span>|<span data-ttu-id="f4d78-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-186">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f4d78-187">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-187">Boolean</span></span>|<span data-ttu-id="f4d78-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-189">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-189">touchIdDisabled</span></span>|<span data-ttu-id="f4d78-190">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-190">Boolean</span></span>|<span data-ttu-id="f4d78-191">Указывает, является ли область настроек сенсорного экрана наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-192">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-192">applePayDisabled</span></span>|<span data-ttu-id="f4d78-193">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-193">Boolean</span></span>|<span data-ttu-id="f4d78-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-195">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-195">zoomDisabled</span></span>|<span data-ttu-id="f4d78-196">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-196">Boolean</span></span>|<span data-ttu-id="f4d78-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-198">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-198">siriDisabled</span></span>|<span data-ttu-id="f4d78-199">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-199">Boolean</span></span>|<span data-ttu-id="f4d78-200">Указывает, наСледуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-201">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-201">diagnosticsDisabled</span></span>|<span data-ttu-id="f4d78-202">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-202">Boolean</span></span>|<span data-ttu-id="f4d78-203">Указывает, является ли область настройки диагностики неактивной, наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-204">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="f4d78-205">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-205">Boolean</span></span>|<span data-ttu-id="f4d78-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-207">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-207">privacyPaneDisabled</span></span>|<span data-ttu-id="f4d78-208">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-208">Boolean</span></span>|<span data-ttu-id="f4d78-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f4d78-210">iTunesPairingMode.</span><span class="sxs-lookup"><span data-stu-id="f4d78-210">iTunesPairingMode</span></span>|<span data-ttu-id="f4d78-211">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="f4d78-211">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="f4d78-212">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="f4d78-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="f4d78-213">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="f4d78-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="f4d78-214">Манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="f4d78-214">managementCertificates</span></span>|<span data-ttu-id="f4d78-215">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="f4d78-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="f4d78-216">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="f4d78-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="f4d78-217">Ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="f4d78-218">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-218">Boolean</span></span>|<span data-ttu-id="f4d78-219">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="f4d78-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="f4d78-220">Аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="f4d78-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="f4d78-221">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-221">Boolean</span></span>|<span data-ttu-id="f4d78-222">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="f4d78-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="f4d78-223">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="f4d78-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="f4d78-224">Int32</span><span class="sxs-lookup"><span data-stu-id="f4d78-224">Int32</span></span>|<span data-ttu-id="f4d78-225">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="f4d78-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="f4d78-226">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="f4d78-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="f4d78-227">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="f4d78-227">enableSharedIPad</span></span>|<span data-ttu-id="f4d78-228">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-228">Boolean</span></span>|<span data-ttu-id="f4d78-229">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="f4d78-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="f4d78-230">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="f4d78-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="f4d78-231">Компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="f4d78-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="f4d78-232">String</span><span class="sxs-lookup"><span data-stu-id="f4d78-232">String</span></span>|<span data-ttu-id="f4d78-233">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="f4d78-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="f4d78-234">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="f4d78-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="f4d78-235">Енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="f4d78-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="f4d78-236">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-236">Boolean</span></span>|<span data-ttu-id="f4d78-237">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="f4d78-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="f4d78-238">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="f4d78-238">Default is false.</span></span> <span data-ttu-id="f4d78-239">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="f4d78-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="f4d78-240">Хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="f4d78-241">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-241">Boolean</span></span>|<span data-ttu-id="f4d78-242">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="f4d78-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="f4d78-243">Имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="f4d78-244">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-244">Boolean</span></span>|<span data-ttu-id="f4d78-245">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="f4d78-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="f4d78-246">Онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="f4d78-247">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-247">Boolean</span></span>|<span data-ttu-id="f4d78-248">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="f4d78-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="f4d78-249">Скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="f4d78-250">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-250">Boolean</span></span>|<span data-ttu-id="f4d78-251">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="f4d78-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="f4d78-252">Симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="f4d78-253">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-253">Boolean</span></span>|<span data-ttu-id="f4d78-254">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="f4d78-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="f4d78-255">Софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="f4d78-256">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-256">Boolean</span></span>|<span data-ttu-id="f4d78-257">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="f4d78-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="f4d78-258">Ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="f4d78-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="f4d78-259">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d78-259">Boolean</span></span>|<span data-ttu-id="f4d78-260">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="f4d78-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="f4d78-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d78-261">Response</span></span>
<span data-ttu-id="f4d78-262">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4d78-262">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4d78-263">Пример</span><span class="sxs-lookup"><span data-stu-id="f4d78-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4d78-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4d78-264">Request</span></span>
<span data-ttu-id="f4d78-265">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4d78-265">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1736

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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="f4d78-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d78-266">Response</span></span>
<span data-ttu-id="f4d78-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4d78-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1785

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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




