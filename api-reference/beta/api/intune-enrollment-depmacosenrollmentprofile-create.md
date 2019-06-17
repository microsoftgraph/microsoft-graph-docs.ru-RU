---
title: Создание Депмакосенроллментпрофиле
description: Создание нового объекта Депмакосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8021d46954b54e34dfa541f87fee95a911caefba
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980273"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="028e4-103">Создание Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="028e4-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="028e4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="028e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="028e4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="028e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="028e4-106">Создание нового объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="028e4-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="028e4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="028e4-107">Prerequisites</span></span>
<span data-ttu-id="028e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="028e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="028e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="028e4-110">Permission type</span></span>|<span data-ttu-id="028e4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="028e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="028e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="028e4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028e4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="028e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="028e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="028e4-115">Not supported.</span></span>|
|<span data-ttu-id="028e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="028e4-116">Application</span></span>|<span data-ttu-id="028e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="028e4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="028e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="028e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="028e4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="028e4-119">Request headers</span></span>
|<span data-ttu-id="028e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="028e4-120">Header</span></span>|<span data-ttu-id="028e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="028e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="028e4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="028e4-122">Authorization</span></span>|<span data-ttu-id="028e4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="028e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="028e4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="028e4-124">Accept</span></span>|<span data-ttu-id="028e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="028e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="028e4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="028e4-126">Request body</span></span>
<span data-ttu-id="028e4-127">В тексте запроса добавьте представление объекта Депмакосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="028e4-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="028e4-128">В следующей таблице приведены свойства, необходимые при создании Депмакосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="028e4-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="028e4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="028e4-129">Property</span></span>|<span data-ttu-id="028e4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="028e4-130">Type</span></span>|<span data-ttu-id="028e4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="028e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="028e4-132">id</span><span class="sxs-lookup"><span data-stu-id="028e4-132">id</span></span>|<span data-ttu-id="028e4-133">String</span><span class="sxs-lookup"><span data-stu-id="028e4-133">String</span></span>|<span data-ttu-id="028e4-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="028e4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="028e4-135">displayName</span></span>|<span data-ttu-id="028e4-136">Строка</span><span class="sxs-lookup"><span data-stu-id="028e4-136">String</span></span>|<span data-ttu-id="028e4-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="028e4-138">description</span><span class="sxs-lookup"><span data-stu-id="028e4-138">description</span></span>|<span data-ttu-id="028e4-139">String</span><span class="sxs-lookup"><span data-stu-id="028e4-139">String</span></span>|<span data-ttu-id="028e4-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="028e4-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="028e4-141">requiresUserAuthentication</span></span>|<span data-ttu-id="028e4-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-142">Boolean</span></span>|<span data-ttu-id="028e4-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="028e4-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="028e4-144">configurationEndpointUrl</span></span>|<span data-ttu-id="028e4-145">String</span><span class="sxs-lookup"><span data-stu-id="028e4-145">String</span></span>|<span data-ttu-id="028e4-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="028e4-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="028e4-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="028e4-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-148">Boolean</span></span>|<span data-ttu-id="028e4-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="028e4-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="028e4-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="028e4-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="028e4-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="028e4-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-152">Boolean</span></span>|<span data-ttu-id="028e4-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="028e4-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="028e4-154">isDefault</span></span>|<span data-ttu-id="028e4-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-155">Boolean</span></span>|<span data-ttu-id="028e4-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-157">supervisedModeEnabled</span></span>|<span data-ttu-id="028e4-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-158">Boolean</span></span>|<span data-ttu-id="028e4-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="028e4-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="028e4-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="028e4-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="028e4-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-162">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="028e4-162">supportDepartment</span></span>|<span data-ttu-id="028e4-163">String</span><span class="sxs-lookup"><span data-stu-id="028e4-163">String</span></span>|<span data-ttu-id="028e4-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-165">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-165">passCodeDisabled</span></span>|<span data-ttu-id="028e4-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-166">Boolean</span></span>|<span data-ttu-id="028e4-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="028e4-168">isMandatory</span></span>|<span data-ttu-id="028e4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-169">Boolean</span></span>|<span data-ttu-id="028e4-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-171">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-171">locationDisabled</span></span>|<span data-ttu-id="028e4-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-172">Boolean</span></span>|<span data-ttu-id="028e4-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-174">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="028e4-174">supportPhoneNumber</span></span>|<span data-ttu-id="028e4-175">String</span><span class="sxs-lookup"><span data-stu-id="028e4-175">String</span></span>|<span data-ttu-id="028e4-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-177">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-177">profileRemovalDisabled</span></span>|<span data-ttu-id="028e4-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-178">Boolean</span></span>|<span data-ttu-id="028e4-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-180">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="028e4-180">restoreBlocked</span></span>|<span data-ttu-id="028e4-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-181">Boolean</span></span>|<span data-ttu-id="028e4-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-183">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-183">appleIdDisabled</span></span>|<span data-ttu-id="028e4-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-184">Boolean</span></span>|<span data-ttu-id="028e4-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-186">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="028e4-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-187">Boolean</span></span>|<span data-ttu-id="028e4-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-189">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-189">touchIdDisabled</span></span>|<span data-ttu-id="028e4-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-190">Boolean</span></span>|<span data-ttu-id="028e4-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-192">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-192">applePayDisabled</span></span>|<span data-ttu-id="028e4-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-193">Boolean</span></span>|<span data-ttu-id="028e4-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-195">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-195">zoomDisabled</span></span>|<span data-ttu-id="028e4-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-196">Boolean</span></span>|<span data-ttu-id="028e4-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-198">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-198">siriDisabled</span></span>|<span data-ttu-id="028e4-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-199">Boolean</span></span>|<span data-ttu-id="028e4-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-201">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-201">diagnosticsDisabled</span></span>|<span data-ttu-id="028e4-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-202">Boolean</span></span>|<span data-ttu-id="028e4-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-204">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="028e4-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-205">Boolean</span></span>|<span data-ttu-id="028e4-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-207">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-207">privacyPaneDisabled</span></span>|<span data-ttu-id="028e4-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-208">Boolean</span></span>|<span data-ttu-id="028e4-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-210">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="028e4-210">deviceNameTemplate</span></span>|<span data-ttu-id="028e4-211">String</span><span class="sxs-lookup"><span data-stu-id="028e4-211">String</span></span>|<span data-ttu-id="028e4-212">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="028e4-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="028e4-213">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="028e4-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="028e4-214">Регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-214">registrationDisabled</span></span>|<span data-ttu-id="028e4-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-215">Boolean</span></span>|<span data-ttu-id="028e4-216">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="028e4-216">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="028e4-217">Филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-217">fileVaultDisabled</span></span>|<span data-ttu-id="028e4-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-218">Boolean</span></span>|<span data-ttu-id="028e4-219">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="028e4-219">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="028e4-220">Иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-220">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="028e4-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-221">Boolean</span></span>|<span data-ttu-id="028e4-222">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="028e4-222">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="028e4-223">Иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-223">iCloudStorageDisabled</span></span>|<span data-ttu-id="028e4-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-224">Boolean</span></span>|<span data-ttu-id="028e4-225">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="028e4-225">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="028e4-226">Чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="028e4-226">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="028e4-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="028e4-227">Boolean</span></span>|<span data-ttu-id="028e4-228">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="028e4-228">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="028e4-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="028e4-229">Response</span></span>
<span data-ttu-id="028e4-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="028e4-230">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="028e4-231">Пример</span><span class="sxs-lookup"><span data-stu-id="028e4-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="028e4-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="028e4-232">Request</span></span>
<span data-ttu-id="028e4-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="028e4-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="028e4-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="028e4-234">Response</span></span>
<span data-ttu-id="028e4-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="028e4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





