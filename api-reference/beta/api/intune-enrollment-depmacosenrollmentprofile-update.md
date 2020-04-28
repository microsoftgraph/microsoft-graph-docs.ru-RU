---
title: Обновление Депмакосенроллментпрофиле
description: Обновление свойств объекта Депмакосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcb5569a055fee4f76aa0977d373731f53dc992d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440962"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="791ff-103">Обновление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="791ff-103">Update depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="791ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="791ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="791ff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="791ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="791ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="791ff-107">Обновление свойств объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="791ff-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="791ff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="791ff-108">Prerequisites</span></span>
<span data-ttu-id="791ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="791ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="791ff-111">Permission type</span></span>|<span data-ttu-id="791ff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="791ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="791ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="791ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="791ff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791ff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="791ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="791ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="791ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791ff-116">Not supported.</span></span>|
|<span data-ttu-id="791ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="791ff-117">Application</span></span>|<span data-ttu-id="791ff-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791ff-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="791ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="791ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="791ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="791ff-120">Request headers</span></span>
|<span data-ttu-id="791ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="791ff-121">Header</span></span>|<span data-ttu-id="791ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="791ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="791ff-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="791ff-123">Authorization</span></span>|<span data-ttu-id="791ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="791ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="791ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="791ff-125">Accept</span></span>|<span data-ttu-id="791ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="791ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="791ff-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="791ff-127">Request body</span></span>
<span data-ttu-id="791ff-128">В тексте запроса добавьте представление объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="791ff-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="791ff-129">В следующей таблице приведены свойства, необходимые при создании [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="791ff-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="791ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="791ff-130">Property</span></span>|<span data-ttu-id="791ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="791ff-131">Type</span></span>|<span data-ttu-id="791ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="791ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="791ff-133">id</span><span class="sxs-lookup"><span data-stu-id="791ff-133">id</span></span>|<span data-ttu-id="791ff-134">String</span><span class="sxs-lookup"><span data-stu-id="791ff-134">String</span></span>|<span data-ttu-id="791ff-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="791ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="791ff-136">displayName</span></span>|<span data-ttu-id="791ff-137">Строка</span><span class="sxs-lookup"><span data-stu-id="791ff-137">String</span></span>|<span data-ttu-id="791ff-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="791ff-139">description</span><span class="sxs-lookup"><span data-stu-id="791ff-139">description</span></span>|<span data-ttu-id="791ff-140">String</span><span class="sxs-lookup"><span data-stu-id="791ff-140">String</span></span>|<span data-ttu-id="791ff-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="791ff-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="791ff-142">requiresUserAuthentication</span></span>|<span data-ttu-id="791ff-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-143">Boolean</span></span>|<span data-ttu-id="791ff-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="791ff-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="791ff-145">configurationEndpointUrl</span></span>|<span data-ttu-id="791ff-146">String</span><span class="sxs-lookup"><span data-stu-id="791ff-146">String</span></span>|<span data-ttu-id="791ff-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="791ff-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="791ff-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="791ff-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-149">Boolean</span></span>|<span data-ttu-id="791ff-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="791ff-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="791ff-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="791ff-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="791ff-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="791ff-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-153">Boolean</span></span>|<span data-ttu-id="791ff-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="791ff-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="791ff-155">isDefault</span></span>|<span data-ttu-id="791ff-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-156">Boolean</span></span>|<span data-ttu-id="791ff-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-158">supervisedModeEnabled</span></span>|<span data-ttu-id="791ff-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-159">Boolean</span></span>|<span data-ttu-id="791ff-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="791ff-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="791ff-161">Дополнительную https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="791ff-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="791ff-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="791ff-163">supportDepartment</span></span>|<span data-ttu-id="791ff-164">String</span><span class="sxs-lookup"><span data-stu-id="791ff-164">String</span></span>|<span data-ttu-id="791ff-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-166">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-166">passCodeDisabled</span></span>|<span data-ttu-id="791ff-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-167">Boolean</span></span>|<span data-ttu-id="791ff-168">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-169">Обязательный</span><span class="sxs-lookup"><span data-stu-id="791ff-169">isMandatory</span></span>|<span data-ttu-id="791ff-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-170">Boolean</span></span>|<span data-ttu-id="791ff-171">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-172">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-172">locationDisabled</span></span>|<span data-ttu-id="791ff-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-173">Boolean</span></span>|<span data-ttu-id="791ff-174">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-175">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="791ff-175">supportPhoneNumber</span></span>|<span data-ttu-id="791ff-176">String</span><span class="sxs-lookup"><span data-stu-id="791ff-176">String</span></span>|<span data-ttu-id="791ff-177">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-178">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-178">profileRemovalDisabled</span></span>|<span data-ttu-id="791ff-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-179">Boolean</span></span>|<span data-ttu-id="791ff-180">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-181">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="791ff-181">restoreBlocked</span></span>|<span data-ttu-id="791ff-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-182">Boolean</span></span>|<span data-ttu-id="791ff-183">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-184">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-184">appleIdDisabled</span></span>|<span data-ttu-id="791ff-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-185">Boolean</span></span>|<span data-ttu-id="791ff-186">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-187">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="791ff-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-188">Boolean</span></span>|<span data-ttu-id="791ff-189">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-190">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-190">touchIdDisabled</span></span>|<span data-ttu-id="791ff-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-191">Boolean</span></span>|<span data-ttu-id="791ff-192">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-193">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-193">applePayDisabled</span></span>|<span data-ttu-id="791ff-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-194">Boolean</span></span>|<span data-ttu-id="791ff-195">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-196">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-196">zoomDisabled</span></span>|<span data-ttu-id="791ff-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-197">Boolean</span></span>|<span data-ttu-id="791ff-198">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-199">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-199">siriDisabled</span></span>|<span data-ttu-id="791ff-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-200">Boolean</span></span>|<span data-ttu-id="791ff-201">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-202">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-202">diagnosticsDisabled</span></span>|<span data-ttu-id="791ff-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-203">Boolean</span></span>|<span data-ttu-id="791ff-204">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-205">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="791ff-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-206">Boolean</span></span>|<span data-ttu-id="791ff-207">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-208">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-208">privacyPaneDisabled</span></span>|<span data-ttu-id="791ff-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-209">Boolean</span></span>|<span data-ttu-id="791ff-210">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-211">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="791ff-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-212">Boolean</span></span>|<span data-ttu-id="791ff-213">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-214">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="791ff-214">deviceNameTemplate</span></span>|<span data-ttu-id="791ff-215">String</span><span class="sxs-lookup"><span data-stu-id="791ff-215">String</span></span>|<span data-ttu-id="791ff-216">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="791ff-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="791ff-217">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-218">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="791ff-218">configurationWebUrl</span></span>|<span data-ttu-id="791ff-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-219">Boolean</span></span>|<span data-ttu-id="791ff-220">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="791ff-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="791ff-221">регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-221">registrationDisabled</span></span>|<span data-ttu-id="791ff-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-222">Boolean</span></span>|<span data-ttu-id="791ff-223">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="791ff-223">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="791ff-224">филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-224">fileVaultDisabled</span></span>|<span data-ttu-id="791ff-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-225">Boolean</span></span>|<span data-ttu-id="791ff-226">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="791ff-226">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="791ff-227">иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-227">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="791ff-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-228">Boolean</span></span>|<span data-ttu-id="791ff-229">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="791ff-229">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="791ff-230">иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="791ff-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-231">Boolean</span></span>|<span data-ttu-id="791ff-232">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="791ff-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="791ff-233">чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="791ff-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="791ff-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="791ff-234">Boolean</span></span>|<span data-ttu-id="791ff-235">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="791ff-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="791ff-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="791ff-236">Response</span></span>
<span data-ttu-id="791ff-237">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="791ff-237">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="791ff-238">Пример</span><span class="sxs-lookup"><span data-stu-id="791ff-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="791ff-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="791ff-239">Request</span></span>
<span data-ttu-id="791ff-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="791ff-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="791ff-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="791ff-241">Response</span></span>
<span data-ttu-id="791ff-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="791ff-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



