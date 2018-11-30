---
title: Обновление depMacOSEnrollmentProfile
description: Обновление свойства объекта depMacOSEnrollmentProfile.
ms.openlocfilehash: 7d0e7a8634d852395fd606e3053e5a2b5609e2a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081769"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="049ca-103">Обновление depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="049ca-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="049ca-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="049ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="049ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="049ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="049ca-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="049ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="049ca-107">Обновление свойства объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="049ca-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="049ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="049ca-108">Prerequisites</span></span>
<span data-ttu-id="049ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="049ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="049ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="049ca-111">Permission type</span></span>|<span data-ttu-id="049ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="049ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="049ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="049ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="049ca-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049ca-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="049ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="049ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="049ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="049ca-116">Not supported.</span></span>|
|<span data-ttu-id="049ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="049ca-117">Application</span></span>|<span data-ttu-id="049ca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="049ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="049ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="049ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="049ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="049ca-120">Request headers</span></span>
|<span data-ttu-id="049ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="049ca-121">Header</span></span>|<span data-ttu-id="049ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="049ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="049ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="049ca-123">Authorization</span></span>|<span data-ttu-id="049ca-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="049ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="049ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="049ca-125">Accept</span></span>|<span data-ttu-id="049ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="049ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="049ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="049ca-127">Request body</span></span>
<span data-ttu-id="049ca-128">В тексте запроса укажите представление JSON для объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="049ca-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="049ca-129">В следующей таблице показаны свойства, которые необходимы для создания [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="049ca-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="049ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="049ca-130">Property</span></span>|<span data-ttu-id="049ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="049ca-131">Type</span></span>|<span data-ttu-id="049ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="049ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="049ca-133">id</span><span class="sxs-lookup"><span data-stu-id="049ca-133">id</span></span>|<span data-ttu-id="049ca-134">String</span><span class="sxs-lookup"><span data-stu-id="049ca-134">String</span></span>|<span data-ttu-id="049ca-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="049ca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="049ca-136">displayName</span></span>|<span data-ttu-id="049ca-137">String</span><span class="sxs-lookup"><span data-stu-id="049ca-137">String</span></span>|<span data-ttu-id="049ca-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="049ca-139">описание</span><span class="sxs-lookup"><span data-stu-id="049ca-139">description</span></span>|<span data-ttu-id="049ca-140">String</span><span class="sxs-lookup"><span data-stu-id="049ca-140">String</span></span>|<span data-ttu-id="049ca-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="049ca-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="049ca-142">requiresUserAuthentication</span></span>|<span data-ttu-id="049ca-143">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-143">Boolean</span></span>|<span data-ttu-id="049ca-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="049ca-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="049ca-145">configurationEndpointUrl</span></span>|<span data-ttu-id="049ca-146">String</span><span class="sxs-lookup"><span data-stu-id="049ca-146">String</span></span>|<span data-ttu-id="049ca-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="049ca-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="049ca-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="049ca-149">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-149">Boolean</span></span>|<span data-ttu-id="049ca-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="049ca-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="049ca-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="049ca-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="049ca-152">isDefault</span></span>|<span data-ttu-id="049ca-153">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-153">Boolean</span></span>|<span data-ttu-id="049ca-154">Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="049ca-155">supervisedModeEnabled</span></span>|<span data-ttu-id="049ca-156">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-156">Boolean</span></span>|<span data-ttu-id="049ca-157">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="049ca-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="049ca-158">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="049ca-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="049ca-159">Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="049ca-160">supportDepartment</span></span>|<span data-ttu-id="049ca-161">String</span><span class="sxs-lookup"><span data-stu-id="049ca-161">String</span></span>|<span data-ttu-id="049ca-162">Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-163">passCodeDisabled</span></span>|<span data-ttu-id="049ca-164">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-164">Boolean</span></span>|<span data-ttu-id="049ca-165">Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="049ca-166">isMandatory</span></span>|<span data-ttu-id="049ca-167">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-167">Boolean</span></span>|<span data-ttu-id="049ca-168">Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-169">locationDisabled</span></span>|<span data-ttu-id="049ca-170">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-170">Boolean</span></span>|<span data-ttu-id="049ca-171">Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="049ca-172">supportPhoneNumber</span></span>|<span data-ttu-id="049ca-173">String</span><span class="sxs-lookup"><span data-stu-id="049ca-173">String</span></span>|<span data-ttu-id="049ca-174">Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-175">profileRemovalDisabled</span></span>|<span data-ttu-id="049ca-176">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-176">Boolean</span></span>|<span data-ttu-id="049ca-177">Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="049ca-178">restoreBlocked</span></span>|<span data-ttu-id="049ca-179">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-179">Boolean</span></span>|<span data-ttu-id="049ca-180">Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-181">appleIdDisabled</span></span>|<span data-ttu-id="049ca-182">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-182">Boolean</span></span>|<span data-ttu-id="049ca-183">Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="049ca-185">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-185">Boolean</span></span>|<span data-ttu-id="049ca-186">Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-187">touchIdDisabled</span></span>|<span data-ttu-id="049ca-188">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-188">Boolean</span></span>|<span data-ttu-id="049ca-189">Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-190">applePayDisabled</span></span>|<span data-ttu-id="049ca-191">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-191">Boolean</span></span>|<span data-ttu-id="049ca-192">Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-193">zoomDisabled</span></span>|<span data-ttu-id="049ca-194">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-194">Boolean</span></span>|<span data-ttu-id="049ca-195">Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-196">siriDisabled</span></span>|<span data-ttu-id="049ca-197">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-197">Boolean</span></span>|<span data-ttu-id="049ca-198">Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-199">diagnosticsDisabled</span></span>|<span data-ttu-id="049ca-200">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-200">Boolean</span></span>|<span data-ttu-id="049ca-201">Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="049ca-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="049ca-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-202">registrationDisabled</span></span>|<span data-ttu-id="049ca-203">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-203">Boolean</span></span>|<span data-ttu-id="049ca-204">Указывает, отключена при регистрации</span><span class="sxs-lookup"><span data-stu-id="049ca-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="049ca-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-205">fileVaultDisabled</span></span>|<span data-ttu-id="049ca-206">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-206">Boolean</span></span>|<span data-ttu-id="049ca-207">Указывает, если отключено хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="049ca-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="049ca-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="049ca-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="049ca-209">Логический</span><span class="sxs-lookup"><span data-stu-id="049ca-209">Boolean</span></span>|<span data-ttu-id="049ca-210">Указывает, если экран анализа iCloud отключен</span><span class="sxs-lookup"><span data-stu-id="049ca-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="049ca-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="049ca-211">Response</span></span>
<span data-ttu-id="049ca-212">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="049ca-212">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="049ca-213">Пример</span><span class="sxs-lookup"><span data-stu-id="049ca-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="049ca-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="049ca-214">Request</span></span>
<span data-ttu-id="049ca-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="049ca-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 864

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="049ca-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="049ca-216">Response</span></span>
<span data-ttu-id="049ca-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="049ca-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```





