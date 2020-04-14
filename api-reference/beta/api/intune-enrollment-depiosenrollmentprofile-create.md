---
title: Создание Депиосенроллментпрофиле
description: Создание нового объекта Депиосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e88af42bfb50a3d2f21b35b6a1e723956e0e3881
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441476"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="6d2af-103">Создание Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="6d2af-103">Create depIOSEnrollmentProfile</span></span>

<span data-ttu-id="6d2af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d2af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d2af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d2af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d2af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d2af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d2af-107">Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6d2af-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d2af-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d2af-108">Prerequisites</span></span>
<span data-ttu-id="6d2af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d2af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d2af-111">Permission type</span></span>|<span data-ttu-id="6d2af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d2af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d2af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d2af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d2af-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2af-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6d2af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d2af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d2af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d2af-116">Not supported.</span></span>|
|<span data-ttu-id="6d2af-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6d2af-117">Application</span></span>|<span data-ttu-id="6d2af-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d2af-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d2af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d2af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6d2af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6d2af-120">Request headers</span></span>
|<span data-ttu-id="6d2af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d2af-121">Header</span></span>|<span data-ttu-id="6d2af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d2af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d2af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d2af-123">Authorization</span></span>|<span data-ttu-id="6d2af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d2af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d2af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d2af-125">Accept</span></span>|<span data-ttu-id="6d2af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d2af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d2af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d2af-127">Request body</span></span>
<span data-ttu-id="6d2af-128">В тексте запроса добавьте представление объекта Депиосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d2af-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="6d2af-129">В следующей таблице приведены свойства, необходимые при создании Депиосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="6d2af-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="6d2af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d2af-130">Property</span></span>|<span data-ttu-id="6d2af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6d2af-131">Type</span></span>|<span data-ttu-id="6d2af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6d2af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d2af-133">id</span><span class="sxs-lookup"><span data-stu-id="6d2af-133">id</span></span>|<span data-ttu-id="6d2af-134">String</span><span class="sxs-lookup"><span data-stu-id="6d2af-134">String</span></span>|<span data-ttu-id="6d2af-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6d2af-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6d2af-136">displayName</span></span>|<span data-ttu-id="6d2af-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6d2af-137">String</span></span>|<span data-ttu-id="6d2af-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6d2af-139">description</span><span class="sxs-lookup"><span data-stu-id="6d2af-139">description</span></span>|<span data-ttu-id="6d2af-140">String</span><span class="sxs-lookup"><span data-stu-id="6d2af-140">String</span></span>|<span data-ttu-id="6d2af-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6d2af-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="6d2af-142">requiresUserAuthentication</span></span>|<span data-ttu-id="6d2af-143">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-143">Boolean</span></span>|<span data-ttu-id="6d2af-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6d2af-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="6d2af-145">configurationEndpointUrl</span></span>|<span data-ttu-id="6d2af-146">String</span><span class="sxs-lookup"><span data-stu-id="6d2af-146">String</span></span>|<span data-ttu-id="6d2af-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6d2af-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="6d2af-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6d2af-149">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-149">Boolean</span></span>|<span data-ttu-id="6d2af-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="6d2af-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="6d2af-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6d2af-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="6d2af-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="6d2af-153">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-153">Boolean</span></span>|<span data-ttu-id="6d2af-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="6d2af-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="6d2af-155">isDefault</span></span>|<span data-ttu-id="6d2af-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d2af-156">Boolean</span></span>|<span data-ttu-id="6d2af-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-158">supervisedModeEnabled</span></span>|<span data-ttu-id="6d2af-159">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-159">Boolean</span></span>|<span data-ttu-id="6d2af-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="6d2af-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="6d2af-161">Дополнительную https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="6d2af-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="6d2af-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="6d2af-163">supportDepartment</span></span>|<span data-ttu-id="6d2af-164">String</span><span class="sxs-lookup"><span data-stu-id="6d2af-164">String</span></span>|<span data-ttu-id="6d2af-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-166">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-166">passCodeDisabled</span></span>|<span data-ttu-id="6d2af-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-167">Boolean</span></span>|<span data-ttu-id="6d2af-168">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-169">Обязательный</span><span class="sxs-lookup"><span data-stu-id="6d2af-169">isMandatory</span></span>|<span data-ttu-id="6d2af-170">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-170">Boolean</span></span>|<span data-ttu-id="6d2af-171">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-172">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-172">locationDisabled</span></span>|<span data-ttu-id="6d2af-173">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-173">Boolean</span></span>|<span data-ttu-id="6d2af-174">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-175">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="6d2af-175">supportPhoneNumber</span></span>|<span data-ttu-id="6d2af-176">String</span><span class="sxs-lookup"><span data-stu-id="6d2af-176">String</span></span>|<span data-ttu-id="6d2af-177">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-178">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-178">profileRemovalDisabled</span></span>|<span data-ttu-id="6d2af-179">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-179">Boolean</span></span>|<span data-ttu-id="6d2af-180">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-181">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="6d2af-181">restoreBlocked</span></span>|<span data-ttu-id="6d2af-182">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-182">Boolean</span></span>|<span data-ttu-id="6d2af-183">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-184">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-184">appleIdDisabled</span></span>|<span data-ttu-id="6d2af-185">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-185">Boolean</span></span>|<span data-ttu-id="6d2af-186">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-187">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="6d2af-188">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-188">Boolean</span></span>|<span data-ttu-id="6d2af-189">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-190">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-190">touchIdDisabled</span></span>|<span data-ttu-id="6d2af-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-191">Boolean</span></span>|<span data-ttu-id="6d2af-192">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-193">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-193">applePayDisabled</span></span>|<span data-ttu-id="6d2af-194">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-194">Boolean</span></span>|<span data-ttu-id="6d2af-195">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-196">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-196">zoomDisabled</span></span>|<span data-ttu-id="6d2af-197">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-197">Boolean</span></span>|<span data-ttu-id="6d2af-198">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-199">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-199">siriDisabled</span></span>|<span data-ttu-id="6d2af-200">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-200">Boolean</span></span>|<span data-ttu-id="6d2af-201">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-202">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-202">diagnosticsDisabled</span></span>|<span data-ttu-id="6d2af-203">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-203">Boolean</span></span>|<span data-ttu-id="6d2af-204">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-205">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="6d2af-206">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-206">Boolean</span></span>|<span data-ttu-id="6d2af-207">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-208">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-208">privacyPaneDisabled</span></span>|<span data-ttu-id="6d2af-209">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-209">Boolean</span></span>|<span data-ttu-id="6d2af-210">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-211">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="6d2af-212">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-212">Boolean</span></span>|<span data-ttu-id="6d2af-213">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-214">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="6d2af-214">deviceNameTemplate</span></span>|<span data-ttu-id="6d2af-215">String</span><span class="sxs-lookup"><span data-stu-id="6d2af-215">String</span></span>|<span data-ttu-id="6d2af-216">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="6d2af-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="6d2af-217">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-218">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="6d2af-218">configurationWebUrl</span></span>|<span data-ttu-id="6d2af-219">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-219">Boolean</span></span>|<span data-ttu-id="6d2af-220">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="6d2af-221">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="6d2af-221">iTunesPairingMode</span></span>|<span data-ttu-id="6d2af-222">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="6d2af-222">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="6d2af-223">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="6d2af-223">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="6d2af-224">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="6d2af-224">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="6d2af-225">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="6d2af-225">managementCertificates</span></span>|<span data-ttu-id="6d2af-226">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="6d2af-226">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="6d2af-227">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="6d2af-227">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="6d2af-228">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-228">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="6d2af-229">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-229">Boolean</span></span>|<span data-ttu-id="6d2af-230">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="6d2af-230">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="6d2af-231">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="6d2af-231">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="6d2af-232">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-232">Boolean</span></span>|<span data-ttu-id="6d2af-233">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="6d2af-233">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="6d2af-234">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="6d2af-234">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="6d2af-235">Int32</span><span class="sxs-lookup"><span data-stu-id="6d2af-235">Int32</span></span>|<span data-ttu-id="6d2af-236">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="6d2af-236">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="6d2af-237">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="6d2af-237">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="6d2af-238">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="6d2af-238">enableSharedIPad</span></span>|<span data-ttu-id="6d2af-239">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-239">Boolean</span></span>|<span data-ttu-id="6d2af-240">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="6d2af-240">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="6d2af-241">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="6d2af-241">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="6d2af-242">компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="6d2af-242">companyPortalVppTokenId</span></span>|<span data-ttu-id="6d2af-243">String</span><span class="sxs-lookup"><span data-stu-id="6d2af-243">String</span></span>|<span data-ttu-id="6d2af-244">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="6d2af-244">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="6d2af-245">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="6d2af-245">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="6d2af-246">енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="6d2af-246">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="6d2af-247">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-247">Boolean</span></span>|<span data-ttu-id="6d2af-248">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="6d2af-248">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="6d2af-249">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="6d2af-249">Default is false.</span></span> <span data-ttu-id="6d2af-250">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="6d2af-250">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="6d2af-251">хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-251">homeButtonScreenDisabled</span></span>|<span data-ttu-id="6d2af-252">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-252">Boolean</span></span>|<span data-ttu-id="6d2af-253">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="6d2af-253">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="6d2af-254">имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-254">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="6d2af-255">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-255">Boolean</span></span>|<span data-ttu-id="6d2af-256">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="6d2af-256">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="6d2af-257">онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-257">onBoardingScreenDisabled</span></span>|<span data-ttu-id="6d2af-258">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-258">Boolean</span></span>|<span data-ttu-id="6d2af-259">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="6d2af-259">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="6d2af-260">симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-260">simSetupScreenDisabled</span></span>|<span data-ttu-id="6d2af-261">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-261">Boolean</span></span>|<span data-ttu-id="6d2af-262">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="6d2af-262">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="6d2af-263">софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-263">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="6d2af-264">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-264">Boolean</span></span>|<span data-ttu-id="6d2af-265">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="6d2af-265">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="6d2af-266">ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-266">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="6d2af-267">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-267">Boolean</span></span>|<span data-ttu-id="6d2af-268">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="6d2af-268">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="6d2af-269">аппеаранцескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-269">appearanceScreenDisabled</span></span>|<span data-ttu-id="6d2af-270">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-270">Boolean</span></span>|<span data-ttu-id="6d2af-271">Указывает, отключен ли экран Апперанце</span><span class="sxs-lookup"><span data-stu-id="6d2af-271">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="6d2af-272">експресслангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-272">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="6d2af-273">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-273">Boolean</span></span>|<span data-ttu-id="6d2af-274">Указывает, отключен ли экран Express Language</span><span class="sxs-lookup"><span data-stu-id="6d2af-274">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="6d2af-275">преферредлангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-275">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="6d2af-276">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-276">Boolean</span></span>|<span data-ttu-id="6d2af-277">Указывает, отключен ли предпочтительный экран языка</span><span class="sxs-lookup"><span data-stu-id="6d2af-277">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="6d2af-278">девицетодевицемигратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-278">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="6d2af-279">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-279">Boolean</span></span>|<span data-ttu-id="6d2af-280">Указывает, отключена ли миграция устройств для устройств</span><span class="sxs-lookup"><span data-stu-id="6d2af-280">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="6d2af-281">велкомескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="6d2af-281">welcomeScreenDisabled</span></span>|<span data-ttu-id="6d2af-282">Логическое</span><span class="sxs-lookup"><span data-stu-id="6d2af-282">Boolean</span></span>|<span data-ttu-id="6d2af-283">Указывает, отключен ли экран Векломе</span><span class="sxs-lookup"><span data-stu-id="6d2af-283">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="6d2af-284">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d2af-284">Response</span></span>
<span data-ttu-id="6d2af-285">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d2af-285">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d2af-286">Пример</span><span class="sxs-lookup"><span data-stu-id="6d2af-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d2af-287">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d2af-287">Request</span></span>
<span data-ttu-id="6d2af-288">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d2af-288">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="6d2af-289">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d2af-289">Response</span></span>
<span data-ttu-id="6d2af-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d2af-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



