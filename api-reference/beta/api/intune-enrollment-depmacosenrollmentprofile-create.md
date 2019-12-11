---
title: Создание Депмакосенроллментпрофиле
description: Создание нового объекта Депмакосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c3f8230f205db059bce1159726e664938b9b5b1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943966"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="de80e-103">Создание Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="de80e-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="de80e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de80e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de80e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de80e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de80e-106">Создание нового объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="de80e-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de80e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de80e-107">Prerequisites</span></span>
<span data-ttu-id="de80e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de80e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de80e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de80e-110">Permission type</span></span>|<span data-ttu-id="de80e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de80e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de80e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de80e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de80e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de80e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="de80e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de80e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de80e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de80e-115">Not supported.</span></span>|
|<span data-ttu-id="de80e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de80e-116">Application</span></span>|<span data-ttu-id="de80e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de80e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de80e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de80e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="de80e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de80e-119">Request headers</span></span>
|<span data-ttu-id="de80e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de80e-120">Header</span></span>|<span data-ttu-id="de80e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de80e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de80e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de80e-122">Authorization</span></span>|<span data-ttu-id="de80e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de80e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de80e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="de80e-124">Accept</span></span>|<span data-ttu-id="de80e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de80e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de80e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de80e-126">Request body</span></span>
<span data-ttu-id="de80e-127">В тексте запроса добавьте представление объекта Депмакосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de80e-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="de80e-128">В следующей таблице приведены свойства, необходимые при создании Депмакосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="de80e-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="de80e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="de80e-129">Property</span></span>|<span data-ttu-id="de80e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="de80e-130">Type</span></span>|<span data-ttu-id="de80e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="de80e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de80e-132">id</span><span class="sxs-lookup"><span data-stu-id="de80e-132">id</span></span>|<span data-ttu-id="de80e-133">String</span><span class="sxs-lookup"><span data-stu-id="de80e-133">String</span></span>|<span data-ttu-id="de80e-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="de80e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="de80e-135">displayName</span></span>|<span data-ttu-id="de80e-136">Строка</span><span class="sxs-lookup"><span data-stu-id="de80e-136">String</span></span>|<span data-ttu-id="de80e-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="de80e-138">description</span><span class="sxs-lookup"><span data-stu-id="de80e-138">description</span></span>|<span data-ttu-id="de80e-139">String</span><span class="sxs-lookup"><span data-stu-id="de80e-139">String</span></span>|<span data-ttu-id="de80e-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="de80e-141">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="de80e-141">requiresUserAuthentication</span></span>|<span data-ttu-id="de80e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-142">Boolean</span></span>|<span data-ttu-id="de80e-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="de80e-144">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="de80e-144">configurationEndpointUrl</span></span>|<span data-ttu-id="de80e-145">Строка</span><span class="sxs-lookup"><span data-stu-id="de80e-145">String</span></span>|<span data-ttu-id="de80e-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="de80e-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="de80e-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="de80e-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-148">Boolean</span></span>|<span data-ttu-id="de80e-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="de80e-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="de80e-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="de80e-151">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="de80e-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="de80e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-152">Boolean</span></span>|<span data-ttu-id="de80e-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="de80e-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="de80e-154">isDefault</span></span>|<span data-ttu-id="de80e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-155">Boolean</span></span>|<span data-ttu-id="de80e-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-157">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-157">supervisedModeEnabled</span></span>|<span data-ttu-id="de80e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-158">Boolean</span></span>|<span data-ttu-id="de80e-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="de80e-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="de80e-160">Дополнительную https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="de80e-160">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="de80e-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-162">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="de80e-162">supportDepartment</span></span>|<span data-ttu-id="de80e-163">Строка</span><span class="sxs-lookup"><span data-stu-id="de80e-163">String</span></span>|<span data-ttu-id="de80e-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-165">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-165">passCodeDisabled</span></span>|<span data-ttu-id="de80e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-166">Boolean</span></span>|<span data-ttu-id="de80e-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="de80e-168">isMandatory</span></span>|<span data-ttu-id="de80e-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-169">Boolean</span></span>|<span data-ttu-id="de80e-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-171">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-171">locationDisabled</span></span>|<span data-ttu-id="de80e-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-172">Boolean</span></span>|<span data-ttu-id="de80e-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-174">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="de80e-174">supportPhoneNumber</span></span>|<span data-ttu-id="de80e-175">Строка</span><span class="sxs-lookup"><span data-stu-id="de80e-175">String</span></span>|<span data-ttu-id="de80e-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-177">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-177">profileRemovalDisabled</span></span>|<span data-ttu-id="de80e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-178">Boolean</span></span>|<span data-ttu-id="de80e-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-180">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="de80e-180">restoreBlocked</span></span>|<span data-ttu-id="de80e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-181">Boolean</span></span>|<span data-ttu-id="de80e-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-183">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-183">appleIdDisabled</span></span>|<span data-ttu-id="de80e-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-184">Boolean</span></span>|<span data-ttu-id="de80e-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-186">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="de80e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-187">Boolean</span></span>|<span data-ttu-id="de80e-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-189">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-189">touchIdDisabled</span></span>|<span data-ttu-id="de80e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-190">Boolean</span></span>|<span data-ttu-id="de80e-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-192">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-192">applePayDisabled</span></span>|<span data-ttu-id="de80e-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-193">Boolean</span></span>|<span data-ttu-id="de80e-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-195">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-195">zoomDisabled</span></span>|<span data-ttu-id="de80e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-196">Boolean</span></span>|<span data-ttu-id="de80e-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-198">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-198">siriDisabled</span></span>|<span data-ttu-id="de80e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-199">Boolean</span></span>|<span data-ttu-id="de80e-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-201">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-201">diagnosticsDisabled</span></span>|<span data-ttu-id="de80e-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-202">Boolean</span></span>|<span data-ttu-id="de80e-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-204">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="de80e-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-205">Boolean</span></span>|<span data-ttu-id="de80e-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-207">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-207">privacyPaneDisabled</span></span>|<span data-ttu-id="de80e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-208">Boolean</span></span>|<span data-ttu-id="de80e-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-210">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="de80e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-211">Boolean</span></span>|<span data-ttu-id="de80e-212">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-213">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="de80e-213">deviceNameTemplate</span></span>|<span data-ttu-id="de80e-214">Строка</span><span class="sxs-lookup"><span data-stu-id="de80e-214">String</span></span>|<span data-ttu-id="de80e-215">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="de80e-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="de80e-216">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-217">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="de80e-217">configurationWebUrl</span></span>|<span data-ttu-id="de80e-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-218">Boolean</span></span>|<span data-ttu-id="de80e-219">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="de80e-219">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="de80e-220">регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-220">registrationDisabled</span></span>|<span data-ttu-id="de80e-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-221">Boolean</span></span>|<span data-ttu-id="de80e-222">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="de80e-222">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="de80e-223">филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-223">fileVaultDisabled</span></span>|<span data-ttu-id="de80e-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-224">Boolean</span></span>|<span data-ttu-id="de80e-225">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="de80e-225">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="de80e-226">иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-226">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="de80e-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-227">Boolean</span></span>|<span data-ttu-id="de80e-228">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="de80e-228">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="de80e-229">иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-229">iCloudStorageDisabled</span></span>|<span data-ttu-id="de80e-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-230">Boolean</span></span>|<span data-ttu-id="de80e-231">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="de80e-231">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="de80e-232">чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="de80e-232">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="de80e-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="de80e-233">Boolean</span></span>|<span data-ttu-id="de80e-234">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="de80e-234">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="de80e-235">Ответ</span><span class="sxs-lookup"><span data-stu-id="de80e-235">Response</span></span>
<span data-ttu-id="de80e-236">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de80e-236">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de80e-237">Пример</span><span class="sxs-lookup"><span data-stu-id="de80e-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="de80e-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="de80e-238">Request</span></span>
<span data-ttu-id="de80e-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de80e-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="de80e-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="de80e-240">Response</span></span>
<span data-ttu-id="de80e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de80e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





