---
title: Создание Депиосенроллментпрофиле
description: Создание нового объекта Депиосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40e506e89a8810db8c638d388ff311b7a4800b6e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696736"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="05402-103">Создание Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="05402-103">Create depIOSEnrollmentProfile</span></span>

<span data-ttu-id="05402-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05402-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05402-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05402-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05402-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05402-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05402-107">Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="05402-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05402-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="05402-108">Prerequisites</span></span>
<span data-ttu-id="05402-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05402-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05402-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05402-111">Permission type</span></span>|<span data-ttu-id="05402-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05402-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05402-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05402-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05402-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05402-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="05402-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05402-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05402-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05402-116">Not supported.</span></span>|
|<span data-ttu-id="05402-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05402-117">Application</span></span>|<span data-ttu-id="05402-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05402-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05402-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05402-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="05402-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="05402-120">Request headers</span></span>
|<span data-ttu-id="05402-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05402-121">Header</span></span>|<span data-ttu-id="05402-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05402-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05402-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05402-123">Authorization</span></span>|<span data-ttu-id="05402-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05402-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05402-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05402-125">Accept</span></span>|<span data-ttu-id="05402-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05402-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05402-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05402-127">Request body</span></span>
<span data-ttu-id="05402-128">В тексте запроса добавьте представление объекта Депиосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05402-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="05402-129">В следующей таблице приведены свойства, необходимые при создании Депиосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="05402-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="05402-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="05402-130">Property</span></span>|<span data-ttu-id="05402-131">Тип</span><span class="sxs-lookup"><span data-stu-id="05402-131">Type</span></span>|<span data-ttu-id="05402-132">Описание</span><span class="sxs-lookup"><span data-stu-id="05402-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05402-133">id</span><span class="sxs-lookup"><span data-stu-id="05402-133">id</span></span>|<span data-ttu-id="05402-134">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-134">String</span></span>|<span data-ttu-id="05402-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="05402-136">displayName</span><span class="sxs-lookup"><span data-stu-id="05402-136">displayName</span></span>|<span data-ttu-id="05402-137">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-137">String</span></span>|<span data-ttu-id="05402-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="05402-139">description</span><span class="sxs-lookup"><span data-stu-id="05402-139">description</span></span>|<span data-ttu-id="05402-140">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-140">String</span></span>|<span data-ttu-id="05402-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="05402-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="05402-142">requiresUserAuthentication</span></span>|<span data-ttu-id="05402-143">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-143">Boolean</span></span>|<span data-ttu-id="05402-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="05402-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="05402-145">configurationEndpointUrl</span></span>|<span data-ttu-id="05402-146">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-146">String</span></span>|<span data-ttu-id="05402-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="05402-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="05402-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="05402-149">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-149">Boolean</span></span>|<span data-ttu-id="05402-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="05402-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="05402-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="05402-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="05402-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="05402-153">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-153">Boolean</span></span>|<span data-ttu-id="05402-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="05402-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="05402-155">isDefault</span></span>|<span data-ttu-id="05402-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="05402-156">Boolean</span></span>|<span data-ttu-id="05402-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="05402-158">supervisedModeEnabled</span></span>|<span data-ttu-id="05402-159">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-159">Boolean</span></span>|<span data-ttu-id="05402-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="05402-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="05402-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="05402-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="05402-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="05402-163">supportDepartment</span></span>|<span data-ttu-id="05402-164">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-164">String</span></span>|<span data-ttu-id="05402-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-166">Обязательный</span><span class="sxs-lookup"><span data-stu-id="05402-166">isMandatory</span></span>|<span data-ttu-id="05402-167">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-167">Boolean</span></span>|<span data-ttu-id="05402-168">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-169">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-169">locationDisabled</span></span>|<span data-ttu-id="05402-170">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-170">Boolean</span></span>|<span data-ttu-id="05402-171">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-172">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="05402-172">supportPhoneNumber</span></span>|<span data-ttu-id="05402-173">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-173">String</span></span>|<span data-ttu-id="05402-174">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-175">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-175">profileRemovalDisabled</span></span>|<span data-ttu-id="05402-176">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-176">Boolean</span></span>|<span data-ttu-id="05402-177">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-178">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="05402-178">restoreBlocked</span></span>|<span data-ttu-id="05402-179">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-179">Boolean</span></span>|<span data-ttu-id="05402-180">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-181">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-181">appleIdDisabled</span></span>|<span data-ttu-id="05402-182">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-182">Boolean</span></span>|<span data-ttu-id="05402-183">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-184">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="05402-185">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-185">Boolean</span></span>|<span data-ttu-id="05402-186">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-187">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-187">touchIdDisabled</span></span>|<span data-ttu-id="05402-188">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-188">Boolean</span></span>|<span data-ttu-id="05402-189">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-190">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-190">applePayDisabled</span></span>|<span data-ttu-id="05402-191">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-191">Boolean</span></span>|<span data-ttu-id="05402-192">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-193">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-193">siriDisabled</span></span>|<span data-ttu-id="05402-194">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-194">Boolean</span></span>|<span data-ttu-id="05402-195">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-196">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-196">diagnosticsDisabled</span></span>|<span data-ttu-id="05402-197">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-197">Boolean</span></span>|<span data-ttu-id="05402-198">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-199">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="05402-200">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-200">Boolean</span></span>|<span data-ttu-id="05402-201">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-202">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-202">privacyPaneDisabled</span></span>|<span data-ttu-id="05402-203">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-203">Boolean</span></span>|<span data-ttu-id="05402-204">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-205">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="05402-206">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-206">Boolean</span></span>|<span data-ttu-id="05402-207">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-208">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="05402-208">deviceNameTemplate</span></span>|<span data-ttu-id="05402-209">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-209">String</span></span>|<span data-ttu-id="05402-210">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="05402-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="05402-211">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-212">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="05402-212">configurationWebUrl</span></span>|<span data-ttu-id="05402-213">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-213">Boolean</span></span>|<span data-ttu-id="05402-214">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="05402-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="05402-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="05402-215">iTunesPairingMode</span></span>|<span data-ttu-id="05402-216">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="05402-216">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="05402-217">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="05402-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="05402-218">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="05402-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="05402-219">манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="05402-219">managementCertificates</span></span>|<span data-ttu-id="05402-220">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="05402-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="05402-221">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="05402-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="05402-222">ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="05402-223">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-223">Boolean</span></span>|<span data-ttu-id="05402-224">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="05402-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="05402-225">аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="05402-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="05402-226">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-226">Boolean</span></span>|<span data-ttu-id="05402-227">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="05402-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="05402-228">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="05402-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="05402-229">Int32</span><span class="sxs-lookup"><span data-stu-id="05402-229">Int32</span></span>|<span data-ttu-id="05402-230">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="05402-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="05402-231">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="05402-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="05402-232">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="05402-232">enableSharedIPad</span></span>|<span data-ttu-id="05402-233">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-233">Boolean</span></span>|<span data-ttu-id="05402-234">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="05402-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="05402-235">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="05402-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="05402-236">компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="05402-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="05402-237">Строка</span><span class="sxs-lookup"><span data-stu-id="05402-237">String</span></span>|<span data-ttu-id="05402-238">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="05402-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="05402-239">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="05402-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="05402-240">енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="05402-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="05402-241">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-241">Boolean</span></span>|<span data-ttu-id="05402-242">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="05402-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="05402-243">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="05402-243">Default is false.</span></span> <span data-ttu-id="05402-244">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="05402-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="05402-245">хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="05402-246">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-246">Boolean</span></span>|<span data-ttu-id="05402-247">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="05402-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="05402-248">имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="05402-249">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-249">Boolean</span></span>|<span data-ttu-id="05402-250">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="05402-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="05402-251">онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="05402-252">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-252">Boolean</span></span>|<span data-ttu-id="05402-253">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="05402-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="05402-254">симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="05402-255">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-255">Boolean</span></span>|<span data-ttu-id="05402-256">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="05402-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="05402-257">софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="05402-258">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-258">Boolean</span></span>|<span data-ttu-id="05402-259">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="05402-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="05402-260">ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="05402-261">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-261">Boolean</span></span>|<span data-ttu-id="05402-262">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="05402-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="05402-263">аппеаранцескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="05402-264">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-264">Boolean</span></span>|<span data-ttu-id="05402-265">Указывает, отключен ли экран Апперанце</span><span class="sxs-lookup"><span data-stu-id="05402-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="05402-266">експресслангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="05402-267">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-267">Boolean</span></span>|<span data-ttu-id="05402-268">Указывает, отключен ли экран Express Language</span><span class="sxs-lookup"><span data-stu-id="05402-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="05402-269">преферредлангуажескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="05402-270">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-270">Boolean</span></span>|<span data-ttu-id="05402-271">Указывает, отключен ли предпочтительный экран языка</span><span class="sxs-lookup"><span data-stu-id="05402-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="05402-272">девицетодевицемигратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="05402-273">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-273">Boolean</span></span>|<span data-ttu-id="05402-274">Указывает, отключена ли миграция устройств для устройств</span><span class="sxs-lookup"><span data-stu-id="05402-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="05402-275">велкомескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="05402-276">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-276">Boolean</span></span>|<span data-ttu-id="05402-277">Указывает, отключен ли экран Векломе</span><span class="sxs-lookup"><span data-stu-id="05402-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="05402-278">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-278">passCodeDisabled</span></span>|<span data-ttu-id="05402-279">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-279">Boolean</span></span>|<span data-ttu-id="05402-280">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="05402-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="05402-281">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-281">zoomDisabled</span></span>|<span data-ttu-id="05402-282">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-282">Boolean</span></span>|<span data-ttu-id="05402-283">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="05402-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="05402-284">ресторекомплетедскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="05402-285">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-285">Boolean</span></span>|<span data-ttu-id="05402-286">Указывает, отключен ли экран Векломе</span><span class="sxs-lookup"><span data-stu-id="05402-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="05402-287">упдатекомплетескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="05402-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="05402-288">Логический</span><span class="sxs-lookup"><span data-stu-id="05402-288">Boolean</span></span>|<span data-ttu-id="05402-289">Указывает, отключен ли экран Векломе</span><span class="sxs-lookup"><span data-stu-id="05402-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="05402-290">Ответ</span><span class="sxs-lookup"><span data-stu-id="05402-290">Response</span></span>
<span data-ttu-id="05402-291">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05402-291">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05402-292">Пример</span><span class="sxs-lookup"><span data-stu-id="05402-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="05402-293">Запрос</span><span class="sxs-lookup"><span data-stu-id="05402-293">Request</span></span>
<span data-ttu-id="05402-294">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05402-294">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 2108

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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
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
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="05402-295">Отклик</span><span class="sxs-lookup"><span data-stu-id="05402-295">Response</span></span>
<span data-ttu-id="05402-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05402-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2157

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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
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
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```





