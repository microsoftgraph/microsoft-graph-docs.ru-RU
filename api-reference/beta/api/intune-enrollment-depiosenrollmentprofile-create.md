---
title: Создание Депиосенроллментпрофиле
description: Создание нового объекта Депиосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa03e61f1b2ad66aa55ea9dce7aa2ed6c58b5c41
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309725"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="1aca5-103">Создание Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="1aca5-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="1aca5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aca5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aca5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1aca5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aca5-106">Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1aca5-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1aca5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1aca5-107">Prerequisites</span></span>
<span data-ttu-id="1aca5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aca5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aca5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aca5-110">Permission type</span></span>|<span data-ttu-id="1aca5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aca5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aca5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aca5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1aca5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aca5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1aca5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aca5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aca5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aca5-115">Not supported.</span></span>|
|<span data-ttu-id="1aca5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aca5-116">Application</span></span>|<span data-ttu-id="1aca5-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aca5-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aca5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aca5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1aca5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aca5-119">Request headers</span></span>
|<span data-ttu-id="1aca5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1aca5-120">Header</span></span>|<span data-ttu-id="1aca5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1aca5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aca5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1aca5-122">Authorization</span></span>|<span data-ttu-id="1aca5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1aca5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aca5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1aca5-124">Accept</span></span>|<span data-ttu-id="1aca5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1aca5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aca5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1aca5-126">Request body</span></span>
<span data-ttu-id="1aca5-127">В тексте запроса добавьте представление объекта Депиосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1aca5-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="1aca5-128">В следующей таблице приведены свойства, необходимые при создании Депиосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="1aca5-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="1aca5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1aca5-129">Property</span></span>|<span data-ttu-id="1aca5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1aca5-130">Type</span></span>|<span data-ttu-id="1aca5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1aca5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aca5-132">id</span><span class="sxs-lookup"><span data-stu-id="1aca5-132">id</span></span>|<span data-ttu-id="1aca5-133">String</span><span class="sxs-lookup"><span data-stu-id="1aca5-133">String</span></span>|<span data-ttu-id="1aca5-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1aca5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1aca5-135">displayName</span></span>|<span data-ttu-id="1aca5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="1aca5-136">String</span></span>|<span data-ttu-id="1aca5-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1aca5-138">description</span><span class="sxs-lookup"><span data-stu-id="1aca5-138">description</span></span>|<span data-ttu-id="1aca5-139">String</span><span class="sxs-lookup"><span data-stu-id="1aca5-139">String</span></span>|<span data-ttu-id="1aca5-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1aca5-141">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="1aca5-141">requiresUserAuthentication</span></span>|<span data-ttu-id="1aca5-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-142">Boolean</span></span>|<span data-ttu-id="1aca5-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1aca5-144">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="1aca5-144">configurationEndpointUrl</span></span>|<span data-ttu-id="1aca5-145">String</span><span class="sxs-lookup"><span data-stu-id="1aca5-145">String</span></span>|<span data-ttu-id="1aca5-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1aca5-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="1aca5-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="1aca5-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-148">Boolean</span></span>|<span data-ttu-id="1aca5-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="1aca5-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="1aca5-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1aca5-151">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="1aca5-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="1aca5-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-152">Boolean</span></span>|<span data-ttu-id="1aca5-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1aca5-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="1aca5-154">isDefault</span></span>|<span data-ttu-id="1aca5-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-155">Boolean</span></span>|<span data-ttu-id="1aca5-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-157">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-157">supervisedModeEnabled</span></span>|<span data-ttu-id="1aca5-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-158">Boolean</span></span>|<span data-ttu-id="1aca5-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="1aca5-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="1aca5-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="1aca5-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="1aca5-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-162">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="1aca5-162">supportDepartment</span></span>|<span data-ttu-id="1aca5-163">String</span><span class="sxs-lookup"><span data-stu-id="1aca5-163">String</span></span>|<span data-ttu-id="1aca5-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-165">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-165">passCodeDisabled</span></span>|<span data-ttu-id="1aca5-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-166">Boolean</span></span>|<span data-ttu-id="1aca5-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="1aca5-168">isMandatory</span></span>|<span data-ttu-id="1aca5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-169">Boolean</span></span>|<span data-ttu-id="1aca5-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-171">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-171">locationDisabled</span></span>|<span data-ttu-id="1aca5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-172">Boolean</span></span>|<span data-ttu-id="1aca5-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-174">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="1aca5-174">supportPhoneNumber</span></span>|<span data-ttu-id="1aca5-175">String</span><span class="sxs-lookup"><span data-stu-id="1aca5-175">String</span></span>|<span data-ttu-id="1aca5-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-177">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-177">profileRemovalDisabled</span></span>|<span data-ttu-id="1aca5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-178">Boolean</span></span>|<span data-ttu-id="1aca5-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-180">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="1aca5-180">restoreBlocked</span></span>|<span data-ttu-id="1aca5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-181">Boolean</span></span>|<span data-ttu-id="1aca5-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-183">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-183">appleIdDisabled</span></span>|<span data-ttu-id="1aca5-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-184">Boolean</span></span>|<span data-ttu-id="1aca5-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-186">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="1aca5-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-187">Boolean</span></span>|<span data-ttu-id="1aca5-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-189">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-189">touchIdDisabled</span></span>|<span data-ttu-id="1aca5-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-190">Boolean</span></span>|<span data-ttu-id="1aca5-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-192">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-192">applePayDisabled</span></span>|<span data-ttu-id="1aca5-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-193">Boolean</span></span>|<span data-ttu-id="1aca5-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-195">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-195">zoomDisabled</span></span>|<span data-ttu-id="1aca5-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-196">Boolean</span></span>|<span data-ttu-id="1aca5-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-198">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-198">siriDisabled</span></span>|<span data-ttu-id="1aca5-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-199">Boolean</span></span>|<span data-ttu-id="1aca5-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-201">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-201">diagnosticsDisabled</span></span>|<span data-ttu-id="1aca5-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-202">Boolean</span></span>|<span data-ttu-id="1aca5-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-204">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="1aca5-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-205">Boolean</span></span>|<span data-ttu-id="1aca5-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-207">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-207">privacyPaneDisabled</span></span>|<span data-ttu-id="1aca5-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-208">Boolean</span></span>|<span data-ttu-id="1aca5-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-210">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="1aca5-210">deviceNameTemplate</span></span>|<span data-ttu-id="1aca5-211">String</span><span class="sxs-lookup"><span data-stu-id="1aca5-211">String</span></span>|<span data-ttu-id="1aca5-212">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="1aca5-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="1aca5-213">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1aca5-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="1aca5-214">iTunesPairingMode</span></span>|<span data-ttu-id="1aca5-215">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="1aca5-215">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="1aca5-216">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="1aca5-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="1aca5-217">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="1aca5-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="1aca5-218">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="1aca5-218">managementCertificates</span></span>|<span data-ttu-id="1aca5-219">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="1aca5-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="1aca5-220">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="1aca5-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="1aca5-221">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="1aca5-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-222">Boolean</span></span>|<span data-ttu-id="1aca5-223">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="1aca5-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="1aca5-224">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="1aca5-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="1aca5-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-225">Boolean</span></span>|<span data-ttu-id="1aca5-226">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="1aca5-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="1aca5-227">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="1aca5-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="1aca5-228">Int32</span><span class="sxs-lookup"><span data-stu-id="1aca5-228">Int32</span></span>|<span data-ttu-id="1aca5-229">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="1aca5-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="1aca5-230">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="1aca5-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="1aca5-231">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="1aca5-231">enableSharedIPad</span></span>|<span data-ttu-id="1aca5-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-232">Boolean</span></span>|<span data-ttu-id="1aca5-233">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="1aca5-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="1aca5-234">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="1aca5-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="1aca5-235">компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="1aca5-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="1aca5-236">String</span><span class="sxs-lookup"><span data-stu-id="1aca5-236">String</span></span>|<span data-ttu-id="1aca5-237">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="1aca5-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="1aca5-238">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="1aca5-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="1aca5-239">енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="1aca5-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="1aca5-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-240">Boolean</span></span>|<span data-ttu-id="1aca5-241">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="1aca5-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="1aca5-242">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="1aca5-242">Default is false.</span></span> <span data-ttu-id="1aca5-243">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="1aca5-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="1aca5-244">хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="1aca5-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-245">Boolean</span></span>|<span data-ttu-id="1aca5-246">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="1aca5-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="1aca5-247">имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="1aca5-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-248">Boolean</span></span>|<span data-ttu-id="1aca5-249">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="1aca5-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="1aca5-250">онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="1aca5-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-251">Boolean</span></span>|<span data-ttu-id="1aca5-252">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="1aca5-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="1aca5-253">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="1aca5-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-254">Boolean</span></span>|<span data-ttu-id="1aca5-255">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="1aca5-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="1aca5-256">симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="1aca5-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-257">Boolean</span></span>|<span data-ttu-id="1aca5-258">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="1aca5-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="1aca5-259">софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="1aca5-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-260">Boolean</span></span>|<span data-ttu-id="1aca5-261">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="1aca5-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="1aca5-262">ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="1aca5-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="1aca5-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aca5-263">Boolean</span></span>|<span data-ttu-id="1aca5-264">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="1aca5-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="1aca5-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aca5-265">Response</span></span>
<span data-ttu-id="1aca5-266">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1aca5-266">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aca5-267">Пример</span><span class="sxs-lookup"><span data-stu-id="1aca5-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aca5-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aca5-268">Request</span></span>
<span data-ttu-id="1aca5-269">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1aca5-269">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1aca5-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aca5-270">Response</span></span>
<span data-ttu-id="1aca5-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1aca5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






