---
title: Обновление Депмакосенроллментпрофиле
description: Обновление свойств объекта Депмакосенроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f386801f1edf03544f46f4f730e830ef70130f7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978481"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="2f45a-103">Обновление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="2f45a-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="2f45a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f45a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f45a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f45a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f45a-106">Обновление свойств объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2f45a-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f45a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f45a-107">Prerequisites</span></span>
<span data-ttu-id="2f45a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f45a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f45a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f45a-110">Permission type</span></span>|<span data-ttu-id="2f45a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f45a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f45a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f45a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f45a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f45a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f45a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f45a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f45a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f45a-115">Not supported.</span></span>|
|<span data-ttu-id="2f45a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f45a-116">Application</span></span>|<span data-ttu-id="2f45a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f45a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f45a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f45a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="2f45a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f45a-119">Request headers</span></span>
|<span data-ttu-id="2f45a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f45a-120">Header</span></span>|<span data-ttu-id="2f45a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2f45a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f45a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f45a-122">Authorization</span></span>|<span data-ttu-id="2f45a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f45a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f45a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2f45a-124">Accept</span></span>|<span data-ttu-id="2f45a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f45a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f45a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f45a-126">Request body</span></span>
<span data-ttu-id="2f45a-127">В тексте запроса добавьте представление объекта [Депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f45a-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="2f45a-128">В следующей таблице приведены свойства, необходимые при создании [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2f45a-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="2f45a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f45a-129">Property</span></span>|<span data-ttu-id="2f45a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2f45a-130">Type</span></span>|<span data-ttu-id="2f45a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2f45a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f45a-132">id</span><span class="sxs-lookup"><span data-stu-id="2f45a-132">id</span></span>|<span data-ttu-id="2f45a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2f45a-133">String</span></span>|<span data-ttu-id="2f45a-134">GUID объекта, наСледуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2f45a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2f45a-135">displayName</span></span>|<span data-ttu-id="2f45a-136">String</span><span class="sxs-lookup"><span data-stu-id="2f45a-136">String</span></span>|<span data-ttu-id="2f45a-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2f45a-138">description</span><span class="sxs-lookup"><span data-stu-id="2f45a-138">description</span></span>|<span data-ttu-id="2f45a-139">String</span><span class="sxs-lookup"><span data-stu-id="2f45a-139">String</span></span>|<span data-ttu-id="2f45a-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2f45a-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="2f45a-141">requiresUserAuthentication</span></span>|<span data-ttu-id="2f45a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-142">Boolean</span></span>|<span data-ttu-id="2f45a-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2f45a-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="2f45a-144">configurationEndpointUrl</span></span>|<span data-ttu-id="2f45a-145">String</span><span class="sxs-lookup"><span data-stu-id="2f45a-145">String</span></span>|<span data-ttu-id="2f45a-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2f45a-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2f45a-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="2f45a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-148">Boolean</span></span>|<span data-ttu-id="2f45a-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="2f45a-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="2f45a-150">НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2f45a-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="2f45a-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="2f45a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-152">Boolean</span></span>|<span data-ttu-id="2f45a-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наСледуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2f45a-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="2f45a-154">isDefault</span></span>|<span data-ttu-id="2f45a-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-155">Boolean</span></span>|<span data-ttu-id="2f45a-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-157">supervisedModeEnabled</span></span>|<span data-ttu-id="2f45a-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-158">Boolean</span></span>|<span data-ttu-id="2f45a-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="2f45a-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="2f45a-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="2f45a-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="2f45a-161">НаСледуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-162">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="2f45a-162">supportDepartment</span></span>|<span data-ttu-id="2f45a-163">String</span><span class="sxs-lookup"><span data-stu-id="2f45a-163">String</span></span>|<span data-ttu-id="2f45a-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-165">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-165">passCodeDisabled</span></span>|<span data-ttu-id="2f45a-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-166">Boolean</span></span>|<span data-ttu-id="2f45a-167">Указывает, является ли область настройки секретного кода наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2f45a-168">isMandatory</span></span>|<span data-ttu-id="2f45a-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-169">Boolean</span></span>|<span data-ttu-id="2f45a-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-171">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-171">locationDisabled</span></span>|<span data-ttu-id="2f45a-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-172">Boolean</span></span>|<span data-ttu-id="2f45a-173">Указывает, является ли область настроек службы расположений наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-174">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="2f45a-174">supportPhoneNumber</span></span>|<span data-ttu-id="2f45a-175">String</span><span class="sxs-lookup"><span data-stu-id="2f45a-175">String</span></span>|<span data-ttu-id="2f45a-176">Номер телефона поддержки, наСледуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-177">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-177">profileRemovalDisabled</span></span>|<span data-ttu-id="2f45a-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-178">Boolean</span></span>|<span data-ttu-id="2f45a-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-180">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="2f45a-180">restoreBlocked</span></span>|<span data-ttu-id="2f45a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-181">Boolean</span></span>|<span data-ttu-id="2f45a-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-183">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-183">appleIdDisabled</span></span>|<span data-ttu-id="2f45a-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-184">Boolean</span></span>|<span data-ttu-id="2f45a-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-186">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="2f45a-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-187">Boolean</span></span>|<span data-ttu-id="2f45a-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-189">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-189">touchIdDisabled</span></span>|<span data-ttu-id="2f45a-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-190">Boolean</span></span>|<span data-ttu-id="2f45a-191">Указывает, является ли область настроек сенсорного экрана наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-192">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-192">applePayDisabled</span></span>|<span data-ttu-id="2f45a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-193">Boolean</span></span>|<span data-ttu-id="2f45a-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-195">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-195">zoomDisabled</span></span>|<span data-ttu-id="2f45a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-196">Boolean</span></span>|<span data-ttu-id="2f45a-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-198">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-198">siriDisabled</span></span>|<span data-ttu-id="2f45a-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-199">Boolean</span></span>|<span data-ttu-id="2f45a-200">Указывает, наСледуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-201">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-201">diagnosticsDisabled</span></span>|<span data-ttu-id="2f45a-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-202">Boolean</span></span>|<span data-ttu-id="2f45a-203">Указывает, является ли область настройки диагностики неактивной, наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-204">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="2f45a-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-205">Boolean</span></span>|<span data-ttu-id="2f45a-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-207">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-207">privacyPaneDisabled</span></span>|<span data-ttu-id="2f45a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-208">Boolean</span></span>|<span data-ttu-id="2f45a-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2f45a-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="2f45a-210">Регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-210">registrationDisabled</span></span>|<span data-ttu-id="2f45a-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-211">Boolean</span></span>|<span data-ttu-id="2f45a-212">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="2f45a-212">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="2f45a-213">Филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-213">fileVaultDisabled</span></span>|<span data-ttu-id="2f45a-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-214">Boolean</span></span>|<span data-ttu-id="2f45a-215">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="2f45a-215">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="2f45a-216">Иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-216">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="2f45a-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-217">Boolean</span></span>|<span data-ttu-id="2f45a-218">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="2f45a-218">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="2f45a-219">Иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-219">iCloudStorageDisabled</span></span>|<span data-ttu-id="2f45a-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-220">Boolean</span></span>|<span data-ttu-id="2f45a-221">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="2f45a-221">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="2f45a-222">Чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="2f45a-222">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="2f45a-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f45a-223">Boolean</span></span>|<span data-ttu-id="2f45a-224">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="2f45a-224">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="2f45a-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f45a-225">Response</span></span>
<span data-ttu-id="2f45a-226">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f45a-226">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f45a-227">Пример</span><span class="sxs-lookup"><span data-stu-id="2f45a-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f45a-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f45a-228">Request</span></span>
<span data-ttu-id="2f45a-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f45a-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1136

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="2f45a-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f45a-230">Response</span></span>
<span data-ttu-id="2f45a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f45a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1185

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```




