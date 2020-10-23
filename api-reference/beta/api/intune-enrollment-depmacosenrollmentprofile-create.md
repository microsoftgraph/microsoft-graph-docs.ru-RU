---
title: Создание Депмакосенроллментпрофиле
description: Создание нового объекта Депмакосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83cf72da8a1e04c2a4226b8433e75b74b8250509
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722587"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="0341f-103">Создание Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0341f-103">Create depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="0341f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0341f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0341f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0341f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0341f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0341f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0341f-107">Создание нового объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0341f-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0341f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0341f-108">Prerequisites</span></span>
<span data-ttu-id="0341f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0341f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0341f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0341f-111">Permission type</span></span>|<span data-ttu-id="0341f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0341f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0341f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0341f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0341f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0341f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0341f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0341f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0341f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0341f-116">Not supported.</span></span>|
|<span data-ttu-id="0341f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0341f-117">Application</span></span>|<span data-ttu-id="0341f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0341f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0341f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0341f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0341f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0341f-120">Request headers</span></span>
|<span data-ttu-id="0341f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0341f-121">Header</span></span>|<span data-ttu-id="0341f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0341f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0341f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0341f-123">Authorization</span></span>|<span data-ttu-id="0341f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0341f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0341f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0341f-125">Accept</span></span>|<span data-ttu-id="0341f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0341f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0341f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0341f-127">Request body</span></span>
<span data-ttu-id="0341f-128">В тексте запроса добавьте представление объекта Депмакосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0341f-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="0341f-129">В следующей таблице приведены свойства, необходимые при создании Депмакосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="0341f-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="0341f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0341f-130">Property</span></span>|<span data-ttu-id="0341f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0341f-131">Type</span></span>|<span data-ttu-id="0341f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0341f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0341f-133">id</span><span class="sxs-lookup"><span data-stu-id="0341f-133">id</span></span>|<span data-ttu-id="0341f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0341f-134">String</span></span>|<span data-ttu-id="0341f-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0341f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0341f-136">displayName</span></span>|<span data-ttu-id="0341f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0341f-137">String</span></span>|<span data-ttu-id="0341f-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0341f-139">description</span><span class="sxs-lookup"><span data-stu-id="0341f-139">description</span></span>|<span data-ttu-id="0341f-140">Строка</span><span class="sxs-lookup"><span data-stu-id="0341f-140">String</span></span>|<span data-ttu-id="0341f-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0341f-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="0341f-142">requiresUserAuthentication</span></span>|<span data-ttu-id="0341f-143">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-143">Boolean</span></span>|<span data-ttu-id="0341f-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0341f-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="0341f-145">configurationEndpointUrl</span></span>|<span data-ttu-id="0341f-146">Строка</span><span class="sxs-lookup"><span data-stu-id="0341f-146">String</span></span>|<span data-ttu-id="0341f-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0341f-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="0341f-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="0341f-149">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-149">Boolean</span></span>|<span data-ttu-id="0341f-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="0341f-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="0341f-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0341f-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="0341f-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="0341f-153">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-153">Boolean</span></span>|<span data-ttu-id="0341f-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0341f-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="0341f-155">isDefault</span></span>|<span data-ttu-id="0341f-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="0341f-156">Boolean</span></span>|<span data-ttu-id="0341f-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-158">supervisedModeEnabled</span></span>|<span data-ttu-id="0341f-159">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-159">Boolean</span></span>|<span data-ttu-id="0341f-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="0341f-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="0341f-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="0341f-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="0341f-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="0341f-163">supportDepartment</span></span>|<span data-ttu-id="0341f-164">Строка</span><span class="sxs-lookup"><span data-stu-id="0341f-164">String</span></span>|<span data-ttu-id="0341f-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-166">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0341f-166">isMandatory</span></span>|<span data-ttu-id="0341f-167">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-167">Boolean</span></span>|<span data-ttu-id="0341f-168">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-169">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-169">locationDisabled</span></span>|<span data-ttu-id="0341f-170">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-170">Boolean</span></span>|<span data-ttu-id="0341f-171">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-172">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="0341f-172">supportPhoneNumber</span></span>|<span data-ttu-id="0341f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="0341f-173">String</span></span>|<span data-ttu-id="0341f-174">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-175">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-175">profileRemovalDisabled</span></span>|<span data-ttu-id="0341f-176">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-176">Boolean</span></span>|<span data-ttu-id="0341f-177">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-178">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="0341f-178">restoreBlocked</span></span>|<span data-ttu-id="0341f-179">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-179">Boolean</span></span>|<span data-ttu-id="0341f-180">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-181">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-181">appleIdDisabled</span></span>|<span data-ttu-id="0341f-182">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-182">Boolean</span></span>|<span data-ttu-id="0341f-183">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-184">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="0341f-185">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-185">Boolean</span></span>|<span data-ttu-id="0341f-186">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-187">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-187">touchIdDisabled</span></span>|<span data-ttu-id="0341f-188">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-188">Boolean</span></span>|<span data-ttu-id="0341f-189">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-190">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-190">applePayDisabled</span></span>|<span data-ttu-id="0341f-191">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-191">Boolean</span></span>|<span data-ttu-id="0341f-192">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-193">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-193">siriDisabled</span></span>|<span data-ttu-id="0341f-194">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-194">Boolean</span></span>|<span data-ttu-id="0341f-195">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-196">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-196">diagnosticsDisabled</span></span>|<span data-ttu-id="0341f-197">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-197">Boolean</span></span>|<span data-ttu-id="0341f-198">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-199">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="0341f-200">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-200">Boolean</span></span>|<span data-ttu-id="0341f-201">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-202">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-202">privacyPaneDisabled</span></span>|<span data-ttu-id="0341f-203">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-203">Boolean</span></span>|<span data-ttu-id="0341f-204">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-205">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="0341f-206">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-206">Boolean</span></span>|<span data-ttu-id="0341f-207">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-208">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="0341f-208">deviceNameTemplate</span></span>|<span data-ttu-id="0341f-209">Строка</span><span class="sxs-lookup"><span data-stu-id="0341f-209">String</span></span>|<span data-ttu-id="0341f-210">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="0341f-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="0341f-211">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-212">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="0341f-212">configurationWebUrl</span></span>|<span data-ttu-id="0341f-213">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-213">Boolean</span></span>|<span data-ttu-id="0341f-214">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0341f-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="0341f-215">регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-215">registrationDisabled</span></span>|<span data-ttu-id="0341f-216">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-216">Boolean</span></span>|<span data-ttu-id="0341f-217">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="0341f-217">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="0341f-218">филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-218">fileVaultDisabled</span></span>|<span data-ttu-id="0341f-219">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-219">Boolean</span></span>|<span data-ttu-id="0341f-220">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="0341f-220">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="0341f-221">иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-221">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="0341f-222">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-222">Boolean</span></span>|<span data-ttu-id="0341f-223">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="0341f-223">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="0341f-224">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-224">passCodeDisabled</span></span>|<span data-ttu-id="0341f-225">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-225">Boolean</span></span>|<span data-ttu-id="0341f-226">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="0341f-226">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="0341f-227">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-227">zoomDisabled</span></span>|<span data-ttu-id="0341f-228">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-228">Boolean</span></span>|<span data-ttu-id="0341f-229">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="0341f-229">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="0341f-230">иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="0341f-231">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-231">Boolean</span></span>|<span data-ttu-id="0341f-232">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="0341f-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="0341f-233">чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="0341f-234">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-234">Boolean</span></span>|<span data-ttu-id="0341f-235">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="0341f-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="0341f-236">акцессибилитискриндисаблед</span><span class="sxs-lookup"><span data-stu-id="0341f-236">accessibilityScreenDisabled</span></span>|<span data-ttu-id="0341f-237">Логический</span><span class="sxs-lookup"><span data-stu-id="0341f-237">Boolean</span></span>|<span data-ttu-id="0341f-238">Указывает, отключен ли экран специальных возможностей</span><span class="sxs-lookup"><span data-stu-id="0341f-238">Indicates if Accessibility screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="0341f-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="0341f-239">Response</span></span>
<span data-ttu-id="0341f-240">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0341f-240">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0341f-241">Пример</span><span class="sxs-lookup"><span data-stu-id="0341f-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="0341f-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="0341f-242">Request</span></span>
<span data-ttu-id="0341f-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0341f-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1300

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="0341f-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="0341f-244">Response</span></span>
<span data-ttu-id="0341f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0341f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1349

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true
}
```





