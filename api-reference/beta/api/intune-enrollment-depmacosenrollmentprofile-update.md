---
title: Обновление Депмакосенроллментпрофиле
description: Обновление свойств объекта Депмакосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96c0ce04c6193d8b69d52ee2aa42c6306e47944e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093807"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="9cf41-103">Обновление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="9cf41-103">Update depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="9cf41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cf41-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cf41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf41-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cf41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf41-107">Обновление свойств объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9cf41-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cf41-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9cf41-108">Prerequisites</span></span>
<span data-ttu-id="9cf41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cf41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf41-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cf41-111">Permission type</span></span>|<span data-ttu-id="9cf41-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cf41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cf41-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cf41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cf41-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf41-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9cf41-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cf41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cf41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cf41-116">Not supported.</span></span>|
|<span data-ttu-id="9cf41-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cf41-117">Application</span></span>|<span data-ttu-id="9cf41-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf41-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cf41-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cf41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="9cf41-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9cf41-120">Request headers</span></span>
|<span data-ttu-id="9cf41-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cf41-121">Header</span></span>|<span data-ttu-id="9cf41-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9cf41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cf41-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cf41-123">Authorization</span></span>|<span data-ttu-id="9cf41-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cf41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cf41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9cf41-125">Accept</span></span>|<span data-ttu-id="9cf41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cf41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cf41-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cf41-127">Request body</span></span>
<span data-ttu-id="9cf41-128">В тексте запроса добавьте представление объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cf41-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="9cf41-129">В следующей таблице приведены свойства, необходимые при создании [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9cf41-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="9cf41-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cf41-130">Property</span></span>|<span data-ttu-id="9cf41-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9cf41-131">Type</span></span>|<span data-ttu-id="9cf41-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9cf41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf41-133">id</span><span class="sxs-lookup"><span data-stu-id="9cf41-133">id</span></span>|<span data-ttu-id="9cf41-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf41-134">String</span></span>|<span data-ttu-id="9cf41-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9cf41-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9cf41-136">displayName</span></span>|<span data-ttu-id="9cf41-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf41-137">String</span></span>|<span data-ttu-id="9cf41-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9cf41-139">description</span><span class="sxs-lookup"><span data-stu-id="9cf41-139">description</span></span>|<span data-ttu-id="9cf41-140">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf41-140">String</span></span>|<span data-ttu-id="9cf41-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9cf41-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="9cf41-142">requiresUserAuthentication</span></span>|<span data-ttu-id="9cf41-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-143">Boolean</span></span>|<span data-ttu-id="9cf41-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9cf41-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="9cf41-145">configurationEndpointUrl</span></span>|<span data-ttu-id="9cf41-146">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf41-146">String</span></span>|<span data-ttu-id="9cf41-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9cf41-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="9cf41-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="9cf41-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-149">Boolean</span></span>|<span data-ttu-id="9cf41-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="9cf41-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="9cf41-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9cf41-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="9cf41-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="9cf41-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-153">Boolean</span></span>|<span data-ttu-id="9cf41-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9cf41-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="9cf41-155">isDefault</span></span>|<span data-ttu-id="9cf41-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-156">Boolean</span></span>|<span data-ttu-id="9cf41-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-158">supervisedModeEnabled</span></span>|<span data-ttu-id="9cf41-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-159">Boolean</span></span>|<span data-ttu-id="9cf41-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="9cf41-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="9cf41-161">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="9cf41-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="9cf41-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="9cf41-163">supportDepartment</span></span>|<span data-ttu-id="9cf41-164">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf41-164">String</span></span>|<span data-ttu-id="9cf41-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-166">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-166">passCodeDisabled</span></span>|<span data-ttu-id="9cf41-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-167">Boolean</span></span>|<span data-ttu-id="9cf41-168">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-169">Обязательный</span><span class="sxs-lookup"><span data-stu-id="9cf41-169">isMandatory</span></span>|<span data-ttu-id="9cf41-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-170">Boolean</span></span>|<span data-ttu-id="9cf41-171">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-172">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-172">locationDisabled</span></span>|<span data-ttu-id="9cf41-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-173">Boolean</span></span>|<span data-ttu-id="9cf41-174">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-175">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="9cf41-175">supportPhoneNumber</span></span>|<span data-ttu-id="9cf41-176">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf41-176">String</span></span>|<span data-ttu-id="9cf41-177">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-178">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-178">profileRemovalDisabled</span></span>|<span data-ttu-id="9cf41-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-179">Boolean</span></span>|<span data-ttu-id="9cf41-180">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-181">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="9cf41-181">restoreBlocked</span></span>|<span data-ttu-id="9cf41-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-182">Boolean</span></span>|<span data-ttu-id="9cf41-183">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-184">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-184">appleIdDisabled</span></span>|<span data-ttu-id="9cf41-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-185">Boolean</span></span>|<span data-ttu-id="9cf41-186">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-187">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="9cf41-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-188">Boolean</span></span>|<span data-ttu-id="9cf41-189">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-190">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-190">touchIdDisabled</span></span>|<span data-ttu-id="9cf41-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-191">Boolean</span></span>|<span data-ttu-id="9cf41-192">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-193">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-193">applePayDisabled</span></span>|<span data-ttu-id="9cf41-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-194">Boolean</span></span>|<span data-ttu-id="9cf41-195">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-196">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-196">zoomDisabled</span></span>|<span data-ttu-id="9cf41-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-197">Boolean</span></span>|<span data-ttu-id="9cf41-198">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-199">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-199">siriDisabled</span></span>|<span data-ttu-id="9cf41-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-200">Boolean</span></span>|<span data-ttu-id="9cf41-201">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-202">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-202">diagnosticsDisabled</span></span>|<span data-ttu-id="9cf41-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-203">Boolean</span></span>|<span data-ttu-id="9cf41-204">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-205">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="9cf41-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-206">Boolean</span></span>|<span data-ttu-id="9cf41-207">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-208">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-208">privacyPaneDisabled</span></span>|<span data-ttu-id="9cf41-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-209">Boolean</span></span>|<span data-ttu-id="9cf41-210">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-211">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="9cf41-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-212">Boolean</span></span>|<span data-ttu-id="9cf41-213">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-214">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="9cf41-214">deviceNameTemplate</span></span>|<span data-ttu-id="9cf41-215">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf41-215">String</span></span>|<span data-ttu-id="9cf41-216">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="9cf41-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="9cf41-217">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-218">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="9cf41-218">configurationWebUrl</span></span>|<span data-ttu-id="9cf41-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-219">Boolean</span></span>|<span data-ttu-id="9cf41-220">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9cf41-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="9cf41-221">регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-221">registrationDisabled</span></span>|<span data-ttu-id="9cf41-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-222">Boolean</span></span>|<span data-ttu-id="9cf41-223">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="9cf41-223">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="9cf41-224">филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-224">fileVaultDisabled</span></span>|<span data-ttu-id="9cf41-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-225">Boolean</span></span>|<span data-ttu-id="9cf41-226">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="9cf41-226">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="9cf41-227">иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-227">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="9cf41-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-228">Boolean</span></span>|<span data-ttu-id="9cf41-229">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="9cf41-229">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="9cf41-230">иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="9cf41-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-231">Boolean</span></span>|<span data-ttu-id="9cf41-232">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="9cf41-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="9cf41-233">чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="9cf41-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="9cf41-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cf41-234">Boolean</span></span>|<span data-ttu-id="9cf41-235">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="9cf41-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="9cf41-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cf41-236">Response</span></span>
<span data-ttu-id="9cf41-237">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9cf41-237">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf41-238">Пример</span><span class="sxs-lookup"><span data-stu-id="9cf41-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cf41-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cf41-239">Request</span></span>
<span data-ttu-id="9cf41-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cf41-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="9cf41-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cf41-241">Response</span></span>
<span data-ttu-id="9cf41-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cf41-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






