---
title: Создание Депиосенроллментпрофиле
description: Создание нового объекта Депиосенроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84ef44ead42bff541510fec435e9178db7ba2e5e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787269"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="9b222-103">Создание Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="9b222-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="9b222-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b222-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b222-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b222-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b222-106">Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9b222-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b222-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b222-107">Prerequisites</span></span>
<span data-ttu-id="9b222-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b222-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b222-110">Permission type</span></span>|<span data-ttu-id="9b222-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b222-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b222-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b222-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b222-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b222-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9b222-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b222-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b222-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b222-115">Not supported.</span></span>|
|<span data-ttu-id="9b222-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b222-116">Application</span></span>|<span data-ttu-id="9b222-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b222-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b222-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b222-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9b222-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b222-119">Request headers</span></span>
|<span data-ttu-id="9b222-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b222-120">Header</span></span>|<span data-ttu-id="9b222-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9b222-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b222-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b222-122">Authorization</span></span>|<span data-ttu-id="9b222-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b222-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b222-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9b222-124">Accept</span></span>|<span data-ttu-id="9b222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b222-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b222-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b222-126">Request body</span></span>
<span data-ttu-id="9b222-127">В тексте запроса добавьте представление объекта Депиосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b222-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="9b222-128">В следующей таблице приведены свойства, необходимые при создании Депиосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="9b222-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="9b222-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b222-129">Property</span></span>|<span data-ttu-id="9b222-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9b222-130">Type</span></span>|<span data-ttu-id="9b222-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9b222-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b222-132">id</span><span class="sxs-lookup"><span data-stu-id="9b222-132">id</span></span>|<span data-ttu-id="9b222-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9b222-133">String</span></span>|<span data-ttu-id="9b222-134">GUID объекта, наСледуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9b222-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9b222-135">displayName</span></span>|<span data-ttu-id="9b222-136">String</span><span class="sxs-lookup"><span data-stu-id="9b222-136">String</span></span>|<span data-ttu-id="9b222-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9b222-138">description</span><span class="sxs-lookup"><span data-stu-id="9b222-138">description</span></span>|<span data-ttu-id="9b222-139">String</span><span class="sxs-lookup"><span data-stu-id="9b222-139">String</span></span>|<span data-ttu-id="9b222-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9b222-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="9b222-141">requiresUserAuthentication</span></span>|<span data-ttu-id="9b222-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-142">Boolean</span></span>|<span data-ttu-id="9b222-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9b222-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="9b222-144">configurationEndpointUrl</span></span>|<span data-ttu-id="9b222-145">String</span><span class="sxs-lookup"><span data-stu-id="9b222-145">String</span></span>|<span data-ttu-id="9b222-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9b222-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="9b222-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="9b222-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-148">Boolean</span></span>|<span data-ttu-id="9b222-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="9b222-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="9b222-150">НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9b222-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="9b222-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="9b222-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-152">Boolean</span></span>|<span data-ttu-id="9b222-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наСледуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9b222-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="9b222-154">isDefault</span></span>|<span data-ttu-id="9b222-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-155">Boolean</span></span>|<span data-ttu-id="9b222-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-157">supervisedModeEnabled</span></span>|<span data-ttu-id="9b222-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-158">Boolean</span></span>|<span data-ttu-id="9b222-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="9b222-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="9b222-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="9b222-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="9b222-161">НаСледуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-162">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="9b222-162">supportDepartment</span></span>|<span data-ttu-id="9b222-163">String</span><span class="sxs-lookup"><span data-stu-id="9b222-163">String</span></span>|<span data-ttu-id="9b222-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-165">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-165">passCodeDisabled</span></span>|<span data-ttu-id="9b222-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-166">Boolean</span></span>|<span data-ttu-id="9b222-167">Указывает, является ли область настройки секретного кода наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="9b222-168">isMandatory</span></span>|<span data-ttu-id="9b222-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-169">Boolean</span></span>|<span data-ttu-id="9b222-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-171">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-171">locationDisabled</span></span>|<span data-ttu-id="9b222-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-172">Boolean</span></span>|<span data-ttu-id="9b222-173">Указывает, является ли область настроек службы расположений наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-174">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="9b222-174">supportPhoneNumber</span></span>|<span data-ttu-id="9b222-175">String</span><span class="sxs-lookup"><span data-stu-id="9b222-175">String</span></span>|<span data-ttu-id="9b222-176">Номер телефона поддержки, наСледуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-177">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-177">profileRemovalDisabled</span></span>|<span data-ttu-id="9b222-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-178">Boolean</span></span>|<span data-ttu-id="9b222-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-180">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="9b222-180">restoreBlocked</span></span>|<span data-ttu-id="9b222-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-181">Boolean</span></span>|<span data-ttu-id="9b222-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-183">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-183">appleIdDisabled</span></span>|<span data-ttu-id="9b222-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-184">Boolean</span></span>|<span data-ttu-id="9b222-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-186">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="9b222-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-187">Boolean</span></span>|<span data-ttu-id="9b222-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-189">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-189">touchIdDisabled</span></span>|<span data-ttu-id="9b222-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-190">Boolean</span></span>|<span data-ttu-id="9b222-191">Указывает, является ли область настроек сенсорного экрана наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-192">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-192">applePayDisabled</span></span>|<span data-ttu-id="9b222-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-193">Boolean</span></span>|<span data-ttu-id="9b222-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-195">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-195">zoomDisabled</span></span>|<span data-ttu-id="9b222-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-196">Boolean</span></span>|<span data-ttu-id="9b222-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-198">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-198">siriDisabled</span></span>|<span data-ttu-id="9b222-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-199">Boolean</span></span>|<span data-ttu-id="9b222-200">Указывает, наСледуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-201">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-201">diagnosticsDisabled</span></span>|<span data-ttu-id="9b222-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-202">Boolean</span></span>|<span data-ttu-id="9b222-203">Указывает, является ли область настройки диагностики неактивной, наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-204">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="9b222-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-205">Boolean</span></span>|<span data-ttu-id="9b222-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-207">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-207">privacyPaneDisabled</span></span>|<span data-ttu-id="9b222-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-208">Boolean</span></span>|<span data-ttu-id="9b222-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-210">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="9b222-210">deviceNameTemplate</span></span>|<span data-ttu-id="9b222-211">String</span><span class="sxs-lookup"><span data-stu-id="9b222-211">String</span></span>|<span data-ttu-id="9b222-212">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="9b222-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="9b222-213">НаСледуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9b222-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="9b222-214">iTunesPairingMode</span></span>|[<span data-ttu-id="9b222-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="9b222-215">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="9b222-216">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="9b222-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="9b222-217">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="9b222-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="9b222-218">Манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="9b222-218">managementCertificates</span></span>|<span data-ttu-id="9b222-219">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="9b222-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="9b222-220">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="9b222-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="9b222-221">Ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="9b222-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-222">Boolean</span></span>|<span data-ttu-id="9b222-223">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="9b222-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="9b222-224">Аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="9b222-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="9b222-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-225">Boolean</span></span>|<span data-ttu-id="9b222-226">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="9b222-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="9b222-227">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="9b222-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="9b222-228">Int32</span><span class="sxs-lookup"><span data-stu-id="9b222-228">Int32</span></span>|<span data-ttu-id="9b222-229">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="9b222-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="9b222-230">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="9b222-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="9b222-231">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="9b222-231">enableSharedIPad</span></span>|<span data-ttu-id="9b222-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-232">Boolean</span></span>|<span data-ttu-id="9b222-233">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="9b222-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="9b222-234">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="9b222-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="9b222-235">Компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="9b222-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="9b222-236">String</span><span class="sxs-lookup"><span data-stu-id="9b222-236">String</span></span>|<span data-ttu-id="9b222-237">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="9b222-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="9b222-238">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="9b222-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="9b222-239">Енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="9b222-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="9b222-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-240">Boolean</span></span>|<span data-ttu-id="9b222-241">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="9b222-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="9b222-242">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="9b222-242">Default is false.</span></span> <span data-ttu-id="9b222-243">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="9b222-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="9b222-244">Хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="9b222-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-245">Boolean</span></span>|<span data-ttu-id="9b222-246">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="9b222-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="9b222-247">Имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="9b222-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-248">Boolean</span></span>|<span data-ttu-id="9b222-249">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="9b222-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="9b222-250">Онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="9b222-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-251">Boolean</span></span>|<span data-ttu-id="9b222-252">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="9b222-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="9b222-253">Скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="9b222-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-254">Boolean</span></span>|<span data-ttu-id="9b222-255">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="9b222-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="9b222-256">Симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="9b222-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-257">Boolean</span></span>|<span data-ttu-id="9b222-258">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="9b222-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="9b222-259">Софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="9b222-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-260">Boolean</span></span>|<span data-ttu-id="9b222-261">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="9b222-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="9b222-262">Ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9b222-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="9b222-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b222-263">Boolean</span></span>|<span data-ttu-id="9b222-264">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="9b222-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="9b222-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b222-265">Response</span></span>
<span data-ttu-id="9b222-266">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b222-266">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b222-267">Пример</span><span class="sxs-lookup"><span data-stu-id="9b222-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b222-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b222-268">Request</span></span>
<span data-ttu-id="9b222-269">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b222-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1791

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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="9b222-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b222-270">Response</span></span>
<span data-ttu-id="9b222-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b222-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1840

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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```





