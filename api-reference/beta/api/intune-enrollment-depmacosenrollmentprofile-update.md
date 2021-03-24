---
title: Обновление depMacOSEnrollmentProfile
description: Обновление свойств объекта depMacOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3830625f30ecb81def4b33a68e91999f0a721551
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145896"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="b599d-103">Обновление depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="b599d-103">Update depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="b599d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b599d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b599d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b599d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b599d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b599d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b599d-107">Обновление свойств объекта [depMacOSEnrollmentProfile.](../resources/intune-enrollment-depmacosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b599d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b599d-108">Prerequisites</span></span>
<span data-ttu-id="b599d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b599d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b599d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b599d-111">Permission type</span></span>|<span data-ttu-id="b599d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b599d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b599d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b599d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b599d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b599d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b599d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b599d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b599d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b599d-116">Not supported.</span></span>|
|<span data-ttu-id="b599d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b599d-117">Application</span></span>|<span data-ttu-id="b599d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b599d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b599d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b599d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="b599d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b599d-120">Request headers</span></span>
|<span data-ttu-id="b599d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b599d-121">Header</span></span>|<span data-ttu-id="b599d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b599d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b599d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b599d-123">Authorization</span></span>|<span data-ttu-id="b599d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b599d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b599d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b599d-125">Accept</span></span>|<span data-ttu-id="b599d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b599d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b599d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b599d-127">Request body</span></span>
<span data-ttu-id="b599d-128">В теле запроса поставляем представление JSON для [объекта depMacOSEnrollmentProfile.](../resources/intune-enrollment-depmacosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="b599d-129">В следующей таблице показаны свойства, необходимые при создании [depMacOSEnrollmentProfile.](../resources/intune-enrollment-depmacosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="b599d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b599d-130">Property</span></span>|<span data-ttu-id="b599d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b599d-131">Type</span></span>|<span data-ttu-id="b599d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b599d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b599d-133">id</span><span class="sxs-lookup"><span data-stu-id="b599d-133">id</span></span>|<span data-ttu-id="b599d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b599d-134">String</span></span>|<span data-ttu-id="b599d-135">GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b599d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b599d-136">displayName</span></span>|<span data-ttu-id="b599d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b599d-137">String</span></span>|<span data-ttu-id="b599d-138">Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b599d-139">description</span><span class="sxs-lookup"><span data-stu-id="b599d-139">description</span></span>|<span data-ttu-id="b599d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b599d-140">String</span></span>|<span data-ttu-id="b599d-141">Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b599d-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="b599d-142">requiresUserAuthentication</span></span>|<span data-ttu-id="b599d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-143">Boolean</span></span>|<span data-ttu-id="b599d-144">Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b599d-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="b599d-145">configurationEndpointUrl</span></span>|<span data-ttu-id="b599d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="b599d-146">String</span></span>|<span data-ttu-id="b599d-147">URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b599d-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b599d-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="b599d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-149">Boolean</span></span>|<span data-ttu-id="b599d-150">Указывает на проверку подлинности с помощью помощника установки Apple вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="b599d-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="b599d-151">Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b599d-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="b599d-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="b599d-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-153">Boolean</span></span>|<span data-ttu-id="b599d-154">Указывает, что портал компании необходим для устройств, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b599d-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="b599d-155">isDefault</span></span>|<span data-ttu-id="b599d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-156">Boolean</span></span>|<span data-ttu-id="b599d-157">Указывает, является ли это профилем по умолчанию, унаследованной от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="b599d-158">supervisedModeEnabled</span></span>|<span data-ttu-id="b599d-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-159">Boolean</span></span>|<span data-ttu-id="b599d-160">Режим Под контролем, True, чтобы включить, ложные в противном случае.</span><span class="sxs-lookup"><span data-stu-id="b599d-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="b599d-161">Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях.</span><span class="sxs-lookup"><span data-stu-id="b599d-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="b599d-162">Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="b599d-163">supportDepartment</span></span>|<span data-ttu-id="b599d-164">Строка</span><span class="sxs-lookup"><span data-stu-id="b599d-164">String</span></span>|<span data-ttu-id="b599d-165">Сведения отдела поддержки, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="b599d-166">isMandatory</span></span>|<span data-ttu-id="b599d-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-167">Boolean</span></span>|<span data-ttu-id="b599d-168">Указывает, является ли профиль обязательным, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-169">locationDisabled</span></span>|<span data-ttu-id="b599d-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-170">Boolean</span></span>|<span data-ttu-id="b599d-171">Указывает, отключено ли области установки службы расположения из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b599d-172">supportPhoneNumber</span></span>|<span data-ttu-id="b599d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b599d-173">String</span></span>|<span data-ttu-id="b599d-174">Номер телефона поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-175">profileRemovalDisabled</span></span>|<span data-ttu-id="b599d-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-176">Boolean</span></span>|<span data-ttu-id="b599d-177">Указывает, отключен ли параметр удаления профиля, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b599d-178">restoreBlocked</span></span>|<span data-ttu-id="b599d-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-179">Boolean</span></span>|<span data-ttu-id="b599d-180">Указывает, заблокирована ли настройка области восстановления, наследуемая [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-181">appleIdDisabled</span></span>|<span data-ttu-id="b599d-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-182">Boolean</span></span>|<span data-ttu-id="b599d-183">Указывает, отключена ли система установки apple id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="b599d-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-185">Boolean</span></span>|<span data-ttu-id="b599d-186">Указывает, отключено ли области установки "Условия и условия", унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-187">touchIdDisabled</span></span>|<span data-ttu-id="b599d-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-188">Boolean</span></span>|<span data-ttu-id="b599d-189">Указывает, отключена ли для настройки сенсорного id наследуемая из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-190">applePayDisabled</span></span>|<span data-ttu-id="b599d-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-191">Boolean</span></span>|<span data-ttu-id="b599d-192">Указывает, отключена ли система установки apple pay inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-193">siriDisabled</span></span>|<span data-ttu-id="b599d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-194">Boolean</span></span>|<span data-ttu-id="b599d-195">Указывает, отключена ли настройка siri из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-196">diagnosticsDisabled</span></span>|<span data-ttu-id="b599d-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-197">Boolean</span></span>|<span data-ttu-id="b599d-198">Указывает, отключено ли области настройки диагностики, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="b599d-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-200">Boolean</span></span>|<span data-ttu-id="b599d-201">Указывает, отключен ли экран настройки displaytone, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-202">privacyPaneDisabled</span></span>|<span data-ttu-id="b599d-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-203">Boolean</span></span>|<span data-ttu-id="b599d-204">Указывает, отключен ли экран конфиденциальности, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="b599d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-206">Boolean</span></span>|<span data-ttu-id="b599d-207">Указывает, отключена ли установка расстановки времени на экране, наследуемая [из depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="b599d-208">deviceNameTemplate</span></span>|<span data-ttu-id="b599d-209">Строка</span><span class="sxs-lookup"><span data-stu-id="b599d-209">String</span></span>|<span data-ttu-id="b599d-210">Задает буквальный или имя шаблон.</span><span class="sxs-lookup"><span data-stu-id="b599d-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="b599d-211">Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="b599d-212">configurationWebUrl</span></span>|<span data-ttu-id="b599d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-213">Boolean</span></span>|<span data-ttu-id="b599d-214">URL-адрес для входа помощника установки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b599d-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b599d-215">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-215">registrationDisabled</span></span>|<span data-ttu-id="b599d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-216">Boolean</span></span>|<span data-ttu-id="b599d-217">Указывает, отключена ли регистрация</span><span class="sxs-lookup"><span data-stu-id="b599d-217">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="b599d-218">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-218">fileVaultDisabled</span></span>|<span data-ttu-id="b599d-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-219">Boolean</span></span>|<span data-ttu-id="b599d-220">Указывает, отключен ли хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="b599d-220">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="b599d-221">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-221">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="b599d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-222">Boolean</span></span>|<span data-ttu-id="b599d-223">Указывает, отключен ли экран iCloud Analytics</span><span class="sxs-lookup"><span data-stu-id="b599d-223">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="b599d-224">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-224">passCodeDisabled</span></span>|<span data-ttu-id="b599d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-225">Boolean</span></span>|<span data-ttu-id="b599d-226">Указывает отключение области установки passcode</span><span class="sxs-lookup"><span data-stu-id="b599d-226">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="b599d-227">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-227">zoomDisabled</span></span>|<span data-ttu-id="b599d-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-228">Boolean</span></span>|<span data-ttu-id="b599d-229">Указывает, отключена ли панорама настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="b599d-229">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="b599d-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="b599d-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-231">Boolean</span></span>|<span data-ttu-id="b599d-232">Указывает, отключены ли документы iCloud и экран настольного компьютера</span><span class="sxs-lookup"><span data-stu-id="b599d-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="b599d-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="b599d-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-234">Boolean</span></span>|<span data-ttu-id="b599d-235">Указывает, отключены ли документы iCloud и экран настольного компьютера</span><span class="sxs-lookup"><span data-stu-id="b599d-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="b599d-236">accessibilityScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="b599d-236">accessibilityScreenDisabled</span></span>|<span data-ttu-id="b599d-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b599d-237">Boolean</span></span>|<span data-ttu-id="b599d-238">Указывает, отключен ли экран доступности</span><span class="sxs-lookup"><span data-stu-id="b599d-238">Indicates if Accessibility screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="b599d-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="b599d-239">Response</span></span>
<span data-ttu-id="b599d-240">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b599d-240">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b599d-241">Пример</span><span class="sxs-lookup"><span data-stu-id="b599d-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="b599d-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="b599d-242">Request</span></span>
<span data-ttu-id="b599d-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b599d-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b599d-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="b599d-244">Response</span></span>
<span data-ttu-id="b599d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b599d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




