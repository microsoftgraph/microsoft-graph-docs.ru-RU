---
title: Обновление depIOSEnrollmentProfile
description: Обновление свойств объекта depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6052f3896e6f9311034b1ea2efcb0e1f084cb18a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135791"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="bea67-103">Обновление depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bea67-103">Update depIOSEnrollmentProfile</span></span>

<span data-ttu-id="bea67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bea67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bea67-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bea67-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bea67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bea67-107">Обновление свойств объекта [depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bea67-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bea67-108">Prerequisites</span></span>
<span data-ttu-id="bea67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bea67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bea67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bea67-111">Permission type</span></span>|<span data-ttu-id="bea67-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bea67-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bea67-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bea67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bea67-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bea67-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bea67-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bea67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bea67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bea67-116">Not supported.</span></span>|
|<span data-ttu-id="bea67-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bea67-117">Application</span></span>|<span data-ttu-id="bea67-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bea67-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bea67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bea67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="bea67-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bea67-120">Request headers</span></span>
|<span data-ttu-id="bea67-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bea67-121">Header</span></span>|<span data-ttu-id="bea67-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bea67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bea67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bea67-123">Authorization</span></span>|<span data-ttu-id="bea67-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bea67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bea67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bea67-125">Accept</span></span>|<span data-ttu-id="bea67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bea67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bea67-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bea67-127">Request body</span></span>
<span data-ttu-id="bea67-128">В теле запроса поставляем представление JSON для объекта [depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="bea67-129">В следующей таблице показаны свойства, необходимые при создании [depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="bea67-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bea67-130">Property</span></span>|<span data-ttu-id="bea67-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bea67-131">Type</span></span>|<span data-ttu-id="bea67-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bea67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bea67-133">id</span><span class="sxs-lookup"><span data-stu-id="bea67-133">id</span></span>|<span data-ttu-id="bea67-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-134">String</span></span>|<span data-ttu-id="bea67-135">GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bea67-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bea67-136">displayName</span></span>|<span data-ttu-id="bea67-137">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-137">String</span></span>|<span data-ttu-id="bea67-138">Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bea67-139">description</span><span class="sxs-lookup"><span data-stu-id="bea67-139">description</span></span>|<span data-ttu-id="bea67-140">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-140">String</span></span>|<span data-ttu-id="bea67-141">Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bea67-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="bea67-142">requiresUserAuthentication</span></span>|<span data-ttu-id="bea67-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-143">Boolean</span></span>|<span data-ttu-id="bea67-144">Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bea67-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="bea67-145">configurationEndpointUrl</span></span>|<span data-ttu-id="bea67-146">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-146">String</span></span>|<span data-ttu-id="bea67-147">URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bea67-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="bea67-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="bea67-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-149">Boolean</span></span>|<span data-ttu-id="bea67-150">Указывает на проверку подлинности с помощью помощника установки Apple вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="bea67-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="bea67-151">Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bea67-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="bea67-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="bea67-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-153">Boolean</span></span>|<span data-ttu-id="bea67-154">Указывает, что портал компании необходим для устройств, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="bea67-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="bea67-155">isDefault</span></span>|<span data-ttu-id="bea67-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-156">Boolean</span></span>|<span data-ttu-id="bea67-157">Указывает, является ли это профилем по умолчанию, унаследованной от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="bea67-158">supervisedModeEnabled</span></span>|<span data-ttu-id="bea67-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-159">Boolean</span></span>|<span data-ttu-id="bea67-160">Режим Под контролем, True, чтобы включить, ложные в противном случае.</span><span class="sxs-lookup"><span data-stu-id="bea67-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="bea67-161">Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях.</span><span class="sxs-lookup"><span data-stu-id="bea67-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="bea67-162">Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="bea67-163">supportDepartment</span></span>|<span data-ttu-id="bea67-164">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-164">String</span></span>|<span data-ttu-id="bea67-165">Сведения отдела поддержки, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="bea67-166">isMandatory</span></span>|<span data-ttu-id="bea67-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-167">Boolean</span></span>|<span data-ttu-id="bea67-168">Указывает, является ли профиль обязательным, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-169">locationDisabled</span></span>|<span data-ttu-id="bea67-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-170">Boolean</span></span>|<span data-ttu-id="bea67-171">Указывает, отключено ли области установки службы расположения из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="bea67-172">supportPhoneNumber</span></span>|<span data-ttu-id="bea67-173">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-173">String</span></span>|<span data-ttu-id="bea67-174">Номер телефона поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-175">profileRemovalDisabled</span></span>|<span data-ttu-id="bea67-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-176">Boolean</span></span>|<span data-ttu-id="bea67-177">Указывает, отключен ли параметр удаления профиля, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="bea67-178">restoreBlocked</span></span>|<span data-ttu-id="bea67-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-179">Boolean</span></span>|<span data-ttu-id="bea67-180">Указывает, заблокирована ли настройка области восстановления, наследуемая [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-181">appleIdDisabled</span></span>|<span data-ttu-id="bea67-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-182">Boolean</span></span>|<span data-ttu-id="bea67-183">Указывает, отключена ли система установки apple id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="bea67-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-185">Boolean</span></span>|<span data-ttu-id="bea67-186">Указывает, отключено ли области установки "Условия и условия", унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-187">touchIdDisabled</span></span>|<span data-ttu-id="bea67-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-188">Boolean</span></span>|<span data-ttu-id="bea67-189">Указывает, отключена ли для настройки сенсорного id наследуемая из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-190">applePayDisabled</span></span>|<span data-ttu-id="bea67-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-191">Boolean</span></span>|<span data-ttu-id="bea67-192">Указывает, отключена ли система установки apple pay inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-193">siriDisabled</span></span>|<span data-ttu-id="bea67-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-194">Boolean</span></span>|<span data-ttu-id="bea67-195">Указывает, отключена ли настройка siri из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-196">diagnosticsDisabled</span></span>|<span data-ttu-id="bea67-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-197">Boolean</span></span>|<span data-ttu-id="bea67-198">Указывает, отключено ли области настройки диагностики, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="bea67-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-200">Boolean</span></span>|<span data-ttu-id="bea67-201">Указывает, отключен ли экран настройки displaytone, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-202">privacyPaneDisabled</span></span>|<span data-ttu-id="bea67-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-203">Boolean</span></span>|<span data-ttu-id="bea67-204">Указывает, отключен ли экран конфиденциальности, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="bea67-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-206">Boolean</span></span>|<span data-ttu-id="bea67-207">Указывает, отключена ли установка расстановки времени на экране, наследуемая [из depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="bea67-208">deviceNameTemplate</span></span>|<span data-ttu-id="bea67-209">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-209">String</span></span>|<span data-ttu-id="bea67-210">Задает буквальный или имя шаблон.</span><span class="sxs-lookup"><span data-stu-id="bea67-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="bea67-211">Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="bea67-212">configurationWebUrl</span></span>|<span data-ttu-id="bea67-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-213">Boolean</span></span>|<span data-ttu-id="bea67-214">URL-адрес для входа помощника установки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bea67-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="bea67-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="bea67-215">iTunesPairingMode</span></span>|<span data-ttu-id="bea67-216">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="bea67-216">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="bea67-217">Указывает режим сопряжения iTunes.</span><span class="sxs-lookup"><span data-stu-id="bea67-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="bea67-218">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="bea67-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="bea67-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="bea67-219">managementCertificates</span></span>|<span data-ttu-id="bea67-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span><span class="sxs-lookup"><span data-stu-id="bea67-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="bea67-221">Сертификаты управления для Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="bea67-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="bea67-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="bea67-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-223">Boolean</span></span>|<span data-ttu-id="bea67-224">Указывает, отключено ли восстановление с Android</span><span class="sxs-lookup"><span data-stu-id="bea67-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="bea67-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="bea67-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="bea67-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-226">Boolean</span></span>|<span data-ttu-id="bea67-227">Указывает, нужно ли устройству ждать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="bea67-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="bea67-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="bea67-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="bea67-229">Int32</span><span class="sxs-lookup"><span data-stu-id="bea67-229">Int32</span></span>|<span data-ttu-id="bea67-230">Это указывает максимальное число пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="bea67-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="bea67-231">Применяется только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="bea67-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="bea67-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="bea67-232">enableSharedIPad</span></span>|<span data-ttu-id="bea67-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-233">Boolean</span></span>|<span data-ttu-id="bea67-234">Это указывает, должно ли устройство быть зарегистрированным в режиме, который включает несколько сценариев пользователей.</span><span class="sxs-lookup"><span data-stu-id="bea67-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="bea67-235">Применимо только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="bea67-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="bea67-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="bea67-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="bea67-237">Строка</span><span class="sxs-lookup"><span data-stu-id="bea67-237">String</span></span>|<span data-ttu-id="bea67-238">Если установлено, указывается, какой маркер Vpp следует использовать для развертывания лицензирования портала компании w/device.</span><span class="sxs-lookup"><span data-stu-id="bea67-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="bea67-239">Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="bea67-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="bea67-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="bea67-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="bea67-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-241">Boolean</span></span>|<span data-ttu-id="bea67-242">Сообщает устройству включить режим одного приложения и применить блокировку приложения во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="bea67-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="bea67-243">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="bea67-243">Default is false.</span></span> <span data-ttu-id="bea67-244">Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal" и "companyPortalVppTokenId".</span><span class="sxs-lookup"><span data-stu-id="bea67-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="bea67-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="bea67-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-246">Boolean</span></span>|<span data-ttu-id="bea67-247">Указывает, отключен ли экран чувствительности домашней кнопки</span><span class="sxs-lookup"><span data-stu-id="bea67-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="bea67-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="bea67-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-249">Boolean</span></span>|<span data-ttu-id="bea67-250">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="bea67-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="bea67-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="bea67-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-252">Boolean</span></span>|<span data-ttu-id="bea67-253">Указывает, отключен ли экран установки бортовой установки</span><span class="sxs-lookup"><span data-stu-id="bea67-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="bea67-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="bea67-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-255">Boolean</span></span>|<span data-ttu-id="bea67-256">Указывает, отключен ли экран SIMSetup</span><span class="sxs-lookup"><span data-stu-id="bea67-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="bea67-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="bea67-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-258">Boolean</span></span>|<span data-ttu-id="bea67-259">Указывает, отключен ли экран обязательного обновления sofware</span><span class="sxs-lookup"><span data-stu-id="bea67-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="bea67-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="bea67-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-261">Boolean</span></span>|<span data-ttu-id="bea67-262">Указывает, отключен ли экран переноса часов</span><span class="sxs-lookup"><span data-stu-id="bea67-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="bea67-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="bea67-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-264">Boolean</span></span>|<span data-ttu-id="bea67-265">Указывает, отключен ли экран Apperance</span><span class="sxs-lookup"><span data-stu-id="bea67-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="bea67-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="bea67-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-267">Boolean</span></span>|<span data-ttu-id="bea67-268">Указывает, отключен ли экран express Language</span><span class="sxs-lookup"><span data-stu-id="bea67-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="bea67-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="bea67-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-270">Boolean</span></span>|<span data-ttu-id="bea67-271">Указывает, отключен ли предпочтительный языковой экран</span><span class="sxs-lookup"><span data-stu-id="bea67-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="bea67-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="bea67-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-273">Boolean</span></span>|<span data-ttu-id="bea67-274">Указывает, отключена ли миграция устройства на устройство</span><span class="sxs-lookup"><span data-stu-id="bea67-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="bea67-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="bea67-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-276">Boolean</span></span>|<span data-ttu-id="bea67-277">Указывает, отключен ли экран Weclome</span><span class="sxs-lookup"><span data-stu-id="bea67-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="bea67-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-278">passCodeDisabled</span></span>|<span data-ttu-id="bea67-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-279">Boolean</span></span>|<span data-ttu-id="bea67-280">Указывает отключение области установки passcode</span><span class="sxs-lookup"><span data-stu-id="bea67-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="bea67-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-281">zoomDisabled</span></span>|<span data-ttu-id="bea67-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-282">Boolean</span></span>|<span data-ttu-id="bea67-283">Указывает, отключена ли панорама настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="bea67-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="bea67-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="bea67-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-285">Boolean</span></span>|<span data-ttu-id="bea67-286">Указывает, отключен ли экран Weclome</span><span class="sxs-lookup"><span data-stu-id="bea67-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="bea67-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="bea67-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="bea67-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="bea67-288">Boolean</span></span>|<span data-ttu-id="bea67-289">Указывает, отключен ли экран Weclome</span><span class="sxs-lookup"><span data-stu-id="bea67-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="bea67-290">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea67-290">Response</span></span>
<span data-ttu-id="bea67-291">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bea67-291">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bea67-292">Пример</span><span class="sxs-lookup"><span data-stu-id="bea67-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="bea67-293">Запрос</span><span class="sxs-lookup"><span data-stu-id="bea67-293">Request</span></span>
<span data-ttu-id="bea67-294">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bea67-294">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="bea67-295">Отклик</span><span class="sxs-lookup"><span data-stu-id="bea67-295">Response</span></span>
<span data-ttu-id="bea67-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bea67-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




