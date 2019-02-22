---
title: Создание Депиосенроллментпрофиле
description: Создание нового объекта Депиосенроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e251217a568ffe0c3e25940ab8300565929861b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174223"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="fdca9-103">Создание Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="fdca9-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="fdca9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdca9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdca9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdca9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdca9-106">Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fdca9-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdca9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fdca9-107">Prerequisites</span></span>
<span data-ttu-id="fdca9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdca9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fdca9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdca9-110">Permission type</span></span>|<span data-ttu-id="fdca9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdca9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdca9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdca9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdca9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdca9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fdca9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdca9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdca9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdca9-115">Not supported.</span></span>|
|<span data-ttu-id="fdca9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdca9-116">Application</span></span>|<span data-ttu-id="fdca9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdca9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdca9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdca9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="fdca9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdca9-119">Request headers</span></span>
|<span data-ttu-id="fdca9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdca9-120">Header</span></span>|<span data-ttu-id="fdca9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fdca9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdca9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdca9-122">Authorization</span></span>|<span data-ttu-id="fdca9-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fdca9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdca9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fdca9-124">Accept</span></span>|<span data-ttu-id="fdca9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fdca9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdca9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdca9-126">Request body</span></span>
<span data-ttu-id="fdca9-127">В тексте запроса добавьте представление объекта Депиосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdca9-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="fdca9-128">В следующей таблице приведены свойства, необходимые при создании Депиосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="fdca9-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="fdca9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdca9-129">Property</span></span>|<span data-ttu-id="fdca9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fdca9-130">Type</span></span>|<span data-ttu-id="fdca9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fdca9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdca9-132">id</span><span class="sxs-lookup"><span data-stu-id="fdca9-132">id</span></span>|<span data-ttu-id="fdca9-133">String</span><span class="sxs-lookup"><span data-stu-id="fdca9-133">String</span></span>|<span data-ttu-id="fdca9-134">GUID объекта, наСледуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdca9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fdca9-135">displayName</span></span>|<span data-ttu-id="fdca9-136">String</span><span class="sxs-lookup"><span data-stu-id="fdca9-136">String</span></span>|<span data-ttu-id="fdca9-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdca9-138">description</span><span class="sxs-lookup"><span data-stu-id="fdca9-138">description</span></span>|<span data-ttu-id="fdca9-139">String</span><span class="sxs-lookup"><span data-stu-id="fdca9-139">String</span></span>|<span data-ttu-id="fdca9-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdca9-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="fdca9-141">requiresUserAuthentication</span></span>|<span data-ttu-id="fdca9-142">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-142">Boolean</span></span>|<span data-ttu-id="fdca9-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdca9-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="fdca9-144">configurationEndpointUrl</span></span>|<span data-ttu-id="fdca9-145">String</span><span class="sxs-lookup"><span data-stu-id="fdca9-145">String</span></span>|<span data-ttu-id="fdca9-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdca9-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="fdca9-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="fdca9-148">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-148">Boolean</span></span>|<span data-ttu-id="fdca9-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="fdca9-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="fdca9-150">НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdca9-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="fdca9-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="fdca9-152">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-152">Boolean</span></span>|<span data-ttu-id="fdca9-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наСледуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdca9-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="fdca9-154">isDefault</span></span>|<span data-ttu-id="fdca9-155">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-155">Boolean</span></span>|<span data-ttu-id="fdca9-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-157">supervisedModeEnabled</span></span>|<span data-ttu-id="fdca9-158">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-158">Boolean</span></span>|<span data-ttu-id="fdca9-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="fdca9-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="fdca9-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="fdca9-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="fdca9-161">НаСледуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-162">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="fdca9-162">supportDepartment</span></span>|<span data-ttu-id="fdca9-163">String</span><span class="sxs-lookup"><span data-stu-id="fdca9-163">String</span></span>|<span data-ttu-id="fdca9-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-165">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-165">passCodeDisabled</span></span>|<span data-ttu-id="fdca9-166">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-166">Boolean</span></span>|<span data-ttu-id="fdca9-167">Указывает, является ли область настройки секретного кода наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fdca9-168">isMandatory</span></span>|<span data-ttu-id="fdca9-169">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-169">Boolean</span></span>|<span data-ttu-id="fdca9-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-171">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-171">locationDisabled</span></span>|<span data-ttu-id="fdca9-172">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-172">Boolean</span></span>|<span data-ttu-id="fdca9-173">Указывает, является ли область настроек службы расположений наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-174">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="fdca9-174">supportPhoneNumber</span></span>|<span data-ttu-id="fdca9-175">String</span><span class="sxs-lookup"><span data-stu-id="fdca9-175">String</span></span>|<span data-ttu-id="fdca9-176">Номер телефона поддержки, наСледуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-177">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-177">profileRemovalDisabled</span></span>|<span data-ttu-id="fdca9-178">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-178">Boolean</span></span>|<span data-ttu-id="fdca9-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-180">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="fdca9-180">restoreBlocked</span></span>|<span data-ttu-id="fdca9-181">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-181">Boolean</span></span>|<span data-ttu-id="fdca9-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-183">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-183">appleIdDisabled</span></span>|<span data-ttu-id="fdca9-184">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-184">Boolean</span></span>|<span data-ttu-id="fdca9-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-186">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="fdca9-187">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-187">Boolean</span></span>|<span data-ttu-id="fdca9-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-189">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-189">touchIdDisabled</span></span>|<span data-ttu-id="fdca9-190">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-190">Boolean</span></span>|<span data-ttu-id="fdca9-191">Указывает, является ли область настроек сенсорного экрана наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-192">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-192">applePayDisabled</span></span>|<span data-ttu-id="fdca9-193">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-193">Boolean</span></span>|<span data-ttu-id="fdca9-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-195">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-195">zoomDisabled</span></span>|<span data-ttu-id="fdca9-196">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-196">Boolean</span></span>|<span data-ttu-id="fdca9-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-198">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-198">siriDisabled</span></span>|<span data-ttu-id="fdca9-199">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-199">Boolean</span></span>|<span data-ttu-id="fdca9-200">Указывает, наСледуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-201">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-201">diagnosticsDisabled</span></span>|<span data-ttu-id="fdca9-202">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-202">Boolean</span></span>|<span data-ttu-id="fdca9-203">Указывает, является ли область настройки диагностики неактивной, наСледуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-204">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="fdca9-205">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-205">Boolean</span></span>|<span data-ttu-id="fdca9-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-207">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-207">privacyPaneDisabled</span></span>|<span data-ttu-id="fdca9-208">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-208">Boolean</span></span>|<span data-ttu-id="fdca9-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdca9-210">iTunesPairingMode.</span><span class="sxs-lookup"><span data-stu-id="fdca9-210">iTunesPairingMode</span></span>|<span data-ttu-id="fdca9-211">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="fdca9-211">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="fdca9-212">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="fdca9-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="fdca9-213">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="fdca9-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="fdca9-214">Манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="fdca9-214">managementCertificates</span></span>|<span data-ttu-id="fdca9-215">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="fdca9-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="fdca9-216">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="fdca9-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="fdca9-217">Ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="fdca9-218">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-218">Boolean</span></span>|<span data-ttu-id="fdca9-219">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="fdca9-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="fdca9-220">Аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="fdca9-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="fdca9-221">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-221">Boolean</span></span>|<span data-ttu-id="fdca9-222">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="fdca9-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="fdca9-223">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="fdca9-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="fdca9-224">Int32</span><span class="sxs-lookup"><span data-stu-id="fdca9-224">Int32</span></span>|<span data-ttu-id="fdca9-225">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="fdca9-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="fdca9-226">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="fdca9-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="fdca9-227">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="fdca9-227">enableSharedIPad</span></span>|<span data-ttu-id="fdca9-228">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-228">Boolean</span></span>|<span data-ttu-id="fdca9-229">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="fdca9-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="fdca9-230">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="fdca9-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="fdca9-231">Компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="fdca9-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="fdca9-232">String</span><span class="sxs-lookup"><span data-stu-id="fdca9-232">String</span></span>|<span data-ttu-id="fdca9-233">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="fdca9-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="fdca9-234">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="fdca9-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="fdca9-235">Енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="fdca9-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="fdca9-236">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-236">Boolean</span></span>|<span data-ttu-id="fdca9-237">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="fdca9-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="fdca9-238">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="fdca9-238">Default is false.</span></span> <span data-ttu-id="fdca9-239">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="fdca9-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="fdca9-240">Хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="fdca9-241">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-241">Boolean</span></span>|<span data-ttu-id="fdca9-242">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="fdca9-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="fdca9-243">Имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="fdca9-244">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-244">Boolean</span></span>|<span data-ttu-id="fdca9-245">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="fdca9-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="fdca9-246">Онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="fdca9-247">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-247">Boolean</span></span>|<span data-ttu-id="fdca9-248">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="fdca9-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="fdca9-249">Скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="fdca9-250">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-250">Boolean</span></span>|<span data-ttu-id="fdca9-251">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="fdca9-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="fdca9-252">Симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="fdca9-253">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-253">Boolean</span></span>|<span data-ttu-id="fdca9-254">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="fdca9-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="fdca9-255">Софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="fdca9-256">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-256">Boolean</span></span>|<span data-ttu-id="fdca9-257">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="fdca9-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="fdca9-258">Ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="fdca9-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="fdca9-259">Логический</span><span class="sxs-lookup"><span data-stu-id="fdca9-259">Boolean</span></span>|<span data-ttu-id="fdca9-260">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="fdca9-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="fdca9-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdca9-261">Response</span></span>
<span data-ttu-id="fdca9-262">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fdca9-262">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdca9-263">Пример</span><span class="sxs-lookup"><span data-stu-id="fdca9-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdca9-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdca9-264">Request</span></span>
<span data-ttu-id="fdca9-265">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdca9-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="fdca9-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdca9-266">Response</span></span>
<span data-ttu-id="fdca9-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdca9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




