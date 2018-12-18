---
title: Обновление depMacOSEnrollmentProfile
description: Обновление свойства объекта depMacOSEnrollmentProfile.
author: tfitzmac
ms.openlocfilehash: 243deaa0724270a9ae152e2c98f831c9d79c825f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350479"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="e02db-103">Обновление depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e02db-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="e02db-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e02db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e02db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e02db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e02db-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e02db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e02db-107">Обновление свойства объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e02db-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e02db-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e02db-108">Prerequisites</span></span>
<span data-ttu-id="e02db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e02db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e02db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e02db-111">Permission type</span></span>|<span data-ttu-id="e02db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e02db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e02db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e02db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e02db-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e02db-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e02db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e02db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e02db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e02db-116">Not supported.</span></span>|
|<span data-ttu-id="e02db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e02db-117">Application</span></span>|<span data-ttu-id="e02db-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e02db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e02db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e02db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="e02db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e02db-120">Request headers</span></span>
|<span data-ttu-id="e02db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e02db-121">Header</span></span>|<span data-ttu-id="e02db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e02db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e02db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e02db-123">Authorization</span></span>|<span data-ttu-id="e02db-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e02db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e02db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e02db-125">Accept</span></span>|<span data-ttu-id="e02db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e02db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e02db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e02db-127">Request body</span></span>
<span data-ttu-id="e02db-128">В тексте запроса укажите представление JSON для объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e02db-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="e02db-129">В следующей таблице показаны свойства, которые необходимы для создания [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e02db-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="e02db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e02db-130">Property</span></span>|<span data-ttu-id="e02db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e02db-131">Type</span></span>|<span data-ttu-id="e02db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e02db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e02db-133">id</span><span class="sxs-lookup"><span data-stu-id="e02db-133">id</span></span>|<span data-ttu-id="e02db-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e02db-134">String</span></span>|<span data-ttu-id="e02db-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e02db-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e02db-136">displayName</span></span>|<span data-ttu-id="e02db-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e02db-137">String</span></span>|<span data-ttu-id="e02db-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e02db-139">описание</span><span class="sxs-lookup"><span data-stu-id="e02db-139">description</span></span>|<span data-ttu-id="e02db-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e02db-140">String</span></span>|<span data-ttu-id="e02db-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e02db-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e02db-142">requiresUserAuthentication</span></span>|<span data-ttu-id="e02db-143">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-143">Boolean</span></span>|<span data-ttu-id="e02db-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e02db-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e02db-145">configurationEndpointUrl</span></span>|<span data-ttu-id="e02db-146">String.</span><span class="sxs-lookup"><span data-stu-id="e02db-146">String</span></span>|<span data-ttu-id="e02db-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e02db-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e02db-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e02db-149">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-149">Boolean</span></span>|<span data-ttu-id="e02db-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="e02db-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="e02db-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e02db-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="e02db-152">isDefault</span></span>|<span data-ttu-id="e02db-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="e02db-153">Boolean</span></span>|<span data-ttu-id="e02db-154">Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="e02db-155">supervisedModeEnabled</span></span>|<span data-ttu-id="e02db-156">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-156">Boolean</span></span>|<span data-ttu-id="e02db-157">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="e02db-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="e02db-158">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="e02db-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="e02db-159">Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="e02db-160">supportDepartment</span></span>|<span data-ttu-id="e02db-161">String.</span><span class="sxs-lookup"><span data-stu-id="e02db-161">String</span></span>|<span data-ttu-id="e02db-162">Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-163">passCodeDisabled</span></span>|<span data-ttu-id="e02db-164">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-164">Boolean</span></span>|<span data-ttu-id="e02db-165">Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="e02db-166">isMandatory</span></span>|<span data-ttu-id="e02db-167">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-167">Boolean</span></span>|<span data-ttu-id="e02db-168">Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-169">locationDisabled</span></span>|<span data-ttu-id="e02db-170">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-170">Boolean</span></span>|<span data-ttu-id="e02db-171">Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e02db-172">supportPhoneNumber</span></span>|<span data-ttu-id="e02db-173">String.</span><span class="sxs-lookup"><span data-stu-id="e02db-173">String</span></span>|<span data-ttu-id="e02db-174">Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-175">profileRemovalDisabled</span></span>|<span data-ttu-id="e02db-176">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-176">Boolean</span></span>|<span data-ttu-id="e02db-177">Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e02db-178">restoreBlocked</span></span>|<span data-ttu-id="e02db-179">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-179">Boolean</span></span>|<span data-ttu-id="e02db-180">Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-181">appleIdDisabled</span></span>|<span data-ttu-id="e02db-182">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-182">Boolean</span></span>|<span data-ttu-id="e02db-183">Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="e02db-185">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-185">Boolean</span></span>|<span data-ttu-id="e02db-186">Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-187">touchIdDisabled</span></span>|<span data-ttu-id="e02db-188">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-188">Boolean</span></span>|<span data-ttu-id="e02db-189">Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-190">applePayDisabled</span></span>|<span data-ttu-id="e02db-191">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-191">Boolean</span></span>|<span data-ttu-id="e02db-192">Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-193">zoomDisabled</span></span>|<span data-ttu-id="e02db-194">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-194">Boolean</span></span>|<span data-ttu-id="e02db-195">Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-196">siriDisabled</span></span>|<span data-ttu-id="e02db-197">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-197">Boolean</span></span>|<span data-ttu-id="e02db-198">Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-199">diagnosticsDisabled</span></span>|<span data-ttu-id="e02db-200">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-200">Boolean</span></span>|<span data-ttu-id="e02db-201">Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e02db-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e02db-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-202">registrationDisabled</span></span>|<span data-ttu-id="e02db-203">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-203">Boolean</span></span>|<span data-ttu-id="e02db-204">Указывает, отключена при регистрации</span><span class="sxs-lookup"><span data-stu-id="e02db-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="e02db-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-205">fileVaultDisabled</span></span>|<span data-ttu-id="e02db-206">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-206">Boolean</span></span>|<span data-ttu-id="e02db-207">Указывает, если отключено хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="e02db-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="e02db-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e02db-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="e02db-209">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e02db-209">Boolean</span></span>|<span data-ttu-id="e02db-210">Указывает, если экран анализа iCloud отключен</span><span class="sxs-lookup"><span data-stu-id="e02db-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="e02db-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="e02db-211">Response</span></span>
<span data-ttu-id="e02db-212">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e02db-212">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e02db-213">Пример</span><span class="sxs-lookup"><span data-stu-id="e02db-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="e02db-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="e02db-214">Request</span></span>
<span data-ttu-id="e02db-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e02db-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e02db-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="e02db-216">Response</span></span>
<span data-ttu-id="e02db-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e02db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





