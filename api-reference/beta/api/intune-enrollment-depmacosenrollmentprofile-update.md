---
title: Обновление Депмакосенроллментпрофиле
description: Обновление свойств объекта Депмакосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6793814258799b4dcbb541c59b14ddfdee1eeb74
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201718"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="cefa5-103">Обновление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="cefa5-103">Update depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="cefa5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cefa5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cefa5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cefa5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cefa5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cefa5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cefa5-107">Обновление свойств объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cefa5-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cefa5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cefa5-108">Prerequisites</span></span>
<span data-ttu-id="cefa5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cefa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cefa5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cefa5-111">Permission type</span></span>|<span data-ttu-id="cefa5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cefa5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cefa5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cefa5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cefa5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefa5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cefa5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cefa5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cefa5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cefa5-116">Not supported.</span></span>|
|<span data-ttu-id="cefa5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cefa5-117">Application</span></span>|<span data-ttu-id="cefa5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefa5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cefa5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cefa5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="cefa5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cefa5-120">Request headers</span></span>
|<span data-ttu-id="cefa5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cefa5-121">Header</span></span>|<span data-ttu-id="cefa5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cefa5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cefa5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cefa5-123">Authorization</span></span>|<span data-ttu-id="cefa5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cefa5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cefa5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cefa5-125">Accept</span></span>|<span data-ttu-id="cefa5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cefa5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cefa5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cefa5-127">Request body</span></span>
<span data-ttu-id="cefa5-128">В тексте запроса добавьте представление объекта [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cefa5-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="cefa5-129">В следующей таблице приведены свойства, необходимые при создании [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="cefa5-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="cefa5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cefa5-130">Property</span></span>|<span data-ttu-id="cefa5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cefa5-131">Type</span></span>|<span data-ttu-id="cefa5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cefa5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cefa5-133">id</span><span class="sxs-lookup"><span data-stu-id="cefa5-133">id</span></span>|<span data-ttu-id="cefa5-134">String</span><span class="sxs-lookup"><span data-stu-id="cefa5-134">String</span></span>|<span data-ttu-id="cefa5-135">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cefa5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cefa5-136">displayName</span></span>|<span data-ttu-id="cefa5-137">String</span><span class="sxs-lookup"><span data-stu-id="cefa5-137">String</span></span>|<span data-ttu-id="cefa5-138">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cefa5-139">description</span><span class="sxs-lookup"><span data-stu-id="cefa5-139">description</span></span>|<span data-ttu-id="cefa5-140">String</span><span class="sxs-lookup"><span data-stu-id="cefa5-140">String</span></span>|<span data-ttu-id="cefa5-141">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cefa5-142">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="cefa5-142">requiresUserAuthentication</span></span>|<span data-ttu-id="cefa5-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-143">Boolean</span></span>|<span data-ttu-id="cefa5-144">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cefa5-145">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="cefa5-145">configurationEndpointUrl</span></span>|<span data-ttu-id="cefa5-146">String</span><span class="sxs-lookup"><span data-stu-id="cefa5-146">String</span></span>|<span data-ttu-id="cefa5-147">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cefa5-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cefa5-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="cefa5-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-149">Boolean</span></span>|<span data-ttu-id="cefa5-150">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="cefa5-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="cefa5-151">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cefa5-152">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="cefa5-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="cefa5-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-153">Boolean</span></span>|<span data-ttu-id="cefa5-154">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="cefa5-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="cefa5-155">isDefault</span></span>|<span data-ttu-id="cefa5-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-156">Boolean</span></span>|<span data-ttu-id="cefa5-157">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-158">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-158">supervisedModeEnabled</span></span>|<span data-ttu-id="cefa5-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-159">Boolean</span></span>|<span data-ttu-id="cefa5-160">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="cefa5-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="cefa5-161"> https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="cefa5-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="cefa5-162">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-163">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="cefa5-163">supportDepartment</span></span>|<span data-ttu-id="cefa5-164">String</span><span class="sxs-lookup"><span data-stu-id="cefa5-164">String</span></span>|<span data-ttu-id="cefa5-165">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-166">Обязательный</span><span class="sxs-lookup"><span data-stu-id="cefa5-166">isMandatory</span></span>|<span data-ttu-id="cefa5-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-167">Boolean</span></span>|<span data-ttu-id="cefa5-168">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-169">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-169">locationDisabled</span></span>|<span data-ttu-id="cefa5-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-170">Boolean</span></span>|<span data-ttu-id="cefa5-171">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-172">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="cefa5-172">supportPhoneNumber</span></span>|<span data-ttu-id="cefa5-173">String</span><span class="sxs-lookup"><span data-stu-id="cefa5-173">String</span></span>|<span data-ttu-id="cefa5-174">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-175">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-175">profileRemovalDisabled</span></span>|<span data-ttu-id="cefa5-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-176">Boolean</span></span>|<span data-ttu-id="cefa5-177">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-178">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="cefa5-178">restoreBlocked</span></span>|<span data-ttu-id="cefa5-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-179">Boolean</span></span>|<span data-ttu-id="cefa5-180">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-181">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-181">appleIdDisabled</span></span>|<span data-ttu-id="cefa5-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-182">Boolean</span></span>|<span data-ttu-id="cefa5-183">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-184">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="cefa5-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-185">Boolean</span></span>|<span data-ttu-id="cefa5-186">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-187">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-187">touchIdDisabled</span></span>|<span data-ttu-id="cefa5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-188">Boolean</span></span>|<span data-ttu-id="cefa5-189">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-190">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-190">applePayDisabled</span></span>|<span data-ttu-id="cefa5-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-191">Boolean</span></span>|<span data-ttu-id="cefa5-192">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-193">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-193">siriDisabled</span></span>|<span data-ttu-id="cefa5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-194">Boolean</span></span>|<span data-ttu-id="cefa5-195">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-196">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-196">diagnosticsDisabled</span></span>|<span data-ttu-id="cefa5-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-197">Boolean</span></span>|<span data-ttu-id="cefa5-198">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-199">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="cefa5-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-200">Boolean</span></span>|<span data-ttu-id="cefa5-201">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-202">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-202">privacyPaneDisabled</span></span>|<span data-ttu-id="cefa5-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-203">Boolean</span></span>|<span data-ttu-id="cefa5-204">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-205">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="cefa5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-206">Boolean</span></span>|<span data-ttu-id="cefa5-207">Указывает, отключена ли настройка времени ожидания экрана от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-208">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="cefa5-208">deviceNameTemplate</span></span>|<span data-ttu-id="cefa5-209">String</span><span class="sxs-lookup"><span data-stu-id="cefa5-209">String</span></span>|<span data-ttu-id="cefa5-210">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="cefa5-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="cefa5-211">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-212">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="cefa5-212">configurationWebUrl</span></span>|<span data-ttu-id="cefa5-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-213">Boolean</span></span>|<span data-ttu-id="cefa5-214">URL-адрес для входа в помощнике по настройке, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cefa5-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="cefa5-215">регистратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-215">registrationDisabled</span></span>|<span data-ttu-id="cefa5-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-216">Boolean</span></span>|<span data-ttu-id="cefa5-217">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="cefa5-217">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="cefa5-218">филеваултдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-218">fileVaultDisabled</span></span>|<span data-ttu-id="cefa5-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-219">Boolean</span></span>|<span data-ttu-id="cefa5-220">Указывает, отключено ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="cefa5-220">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="cefa5-221">иклауддиагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-221">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="cefa5-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-222">Boolean</span></span>|<span data-ttu-id="cefa5-223">Указывает, отключен ли экран аналитики iCloud</span><span class="sxs-lookup"><span data-stu-id="cefa5-223">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="cefa5-224">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-224">passCodeDisabled</span></span>|<span data-ttu-id="cefa5-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-225">Boolean</span></span>|<span data-ttu-id="cefa5-226">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="cefa5-226">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="cefa5-227">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-227">zoomDisabled</span></span>|<span data-ttu-id="cefa5-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-228">Boolean</span></span>|<span data-ttu-id="cefa5-229">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="cefa5-229">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="cefa5-230">иклаудсторажедисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="cefa5-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-231">Boolean</span></span>|<span data-ttu-id="cefa5-232">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="cefa5-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="cefa5-233">чусэйаурлоккскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="cefa5-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-234">Boolean</span></span>|<span data-ttu-id="cefa5-235">Указывает, отключен ли документ iCloud и экран рабочего стола</span><span class="sxs-lookup"><span data-stu-id="cefa5-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="cefa5-236">акцессибилитискриндисаблед</span><span class="sxs-lookup"><span data-stu-id="cefa5-236">accessibilityScreenDisabled</span></span>|<span data-ttu-id="cefa5-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="cefa5-237">Boolean</span></span>|<span data-ttu-id="cefa5-238">Указывает, отключен ли экран специальных возможностей</span><span class="sxs-lookup"><span data-stu-id="cefa5-238">Indicates if Accessibility screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="cefa5-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="cefa5-239">Response</span></span>
<span data-ttu-id="cefa5-240">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cefa5-240">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cefa5-241">Пример</span><span class="sxs-lookup"><span data-stu-id="cefa5-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="cefa5-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="cefa5-242">Request</span></span>
<span data-ttu-id="cefa5-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cefa5-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="cefa5-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="cefa5-244">Response</span></span>
<span data-ttu-id="cefa5-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cefa5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




