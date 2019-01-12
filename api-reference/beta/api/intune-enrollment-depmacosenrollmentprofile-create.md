---
title: Создание depMacOSEnrollmentProfile
description: Создание нового объекта depMacOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f61ace61d1ce06be6d448b221924e4ec8a4f7505
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971328"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="71410-103">Создание depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="71410-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="71410-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71410-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71410-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71410-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71410-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71410-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71410-107">Создание нового объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="71410-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71410-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71410-108">Prerequisites</span></span>
<span data-ttu-id="71410-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71410-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71410-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71410-111">Permission type</span></span>|<span data-ttu-id="71410-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71410-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71410-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71410-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71410-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71410-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="71410-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71410-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71410-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71410-116">Not supported.</span></span>|
|<span data-ttu-id="71410-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71410-117">Application</span></span>|<span data-ttu-id="71410-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71410-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71410-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71410-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="71410-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71410-120">Request headers</span></span>
|<span data-ttu-id="71410-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71410-121">Header</span></span>|<span data-ttu-id="71410-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71410-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71410-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71410-123">Authorization</span></span>|<span data-ttu-id="71410-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="71410-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71410-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71410-125">Accept</span></span>|<span data-ttu-id="71410-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71410-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71410-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71410-127">Request body</span></span>
<span data-ttu-id="71410-128">В тексте запроса укажите представление JSON для объекта depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="71410-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="71410-129">В следующей таблице показаны свойства, которые необходимы для создания depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="71410-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="71410-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71410-130">Property</span></span>|<span data-ttu-id="71410-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71410-131">Type</span></span>|<span data-ttu-id="71410-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71410-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71410-133">id</span><span class="sxs-lookup"><span data-stu-id="71410-133">id</span></span>|<span data-ttu-id="71410-134">Строка</span><span class="sxs-lookup"><span data-stu-id="71410-134">String</span></span>|<span data-ttu-id="71410-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="71410-136">displayName</span><span class="sxs-lookup"><span data-stu-id="71410-136">displayName</span></span>|<span data-ttu-id="71410-137">Строка</span><span class="sxs-lookup"><span data-stu-id="71410-137">String</span></span>|<span data-ttu-id="71410-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="71410-139">описание</span><span class="sxs-lookup"><span data-stu-id="71410-139">description</span></span>|<span data-ttu-id="71410-140">Строка</span><span class="sxs-lookup"><span data-stu-id="71410-140">String</span></span>|<span data-ttu-id="71410-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="71410-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="71410-142">requiresUserAuthentication</span></span>|<span data-ttu-id="71410-143">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-143">Boolean</span></span>|<span data-ttu-id="71410-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="71410-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="71410-145">configurationEndpointUrl</span></span>|<span data-ttu-id="71410-146">Строка</span><span class="sxs-lookup"><span data-stu-id="71410-146">String</span></span>|<span data-ttu-id="71410-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="71410-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="71410-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="71410-149">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-149">Boolean</span></span>|<span data-ttu-id="71410-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="71410-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="71410-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="71410-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="71410-152">isDefault</span></span>|<span data-ttu-id="71410-153">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-153">Boolean</span></span>|<span data-ttu-id="71410-154">Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="71410-155">supervisedModeEnabled</span></span>|<span data-ttu-id="71410-156">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-156">Boolean</span></span>|<span data-ttu-id="71410-157">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="71410-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="71410-158">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="71410-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="71410-159">Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="71410-160">supportDepartment</span></span>|<span data-ttu-id="71410-161">Строка</span><span class="sxs-lookup"><span data-stu-id="71410-161">String</span></span>|<span data-ttu-id="71410-162">Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-163">passCodeDisabled</span></span>|<span data-ttu-id="71410-164">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-164">Boolean</span></span>|<span data-ttu-id="71410-165">Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="71410-166">isMandatory</span></span>|<span data-ttu-id="71410-167">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-167">Boolean</span></span>|<span data-ttu-id="71410-168">Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-169">locationDisabled</span></span>|<span data-ttu-id="71410-170">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-170">Boolean</span></span>|<span data-ttu-id="71410-171">Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="71410-172">supportPhoneNumber</span></span>|<span data-ttu-id="71410-173">Строка</span><span class="sxs-lookup"><span data-stu-id="71410-173">String</span></span>|<span data-ttu-id="71410-174">Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-175">profileRemovalDisabled</span></span>|<span data-ttu-id="71410-176">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-176">Boolean</span></span>|<span data-ttu-id="71410-177">Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="71410-178">restoreBlocked</span></span>|<span data-ttu-id="71410-179">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-179">Boolean</span></span>|<span data-ttu-id="71410-180">Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-181">appleIdDisabled</span></span>|<span data-ttu-id="71410-182">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-182">Boolean</span></span>|<span data-ttu-id="71410-183">Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="71410-185">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-185">Boolean</span></span>|<span data-ttu-id="71410-186">Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-187">touchIdDisabled</span></span>|<span data-ttu-id="71410-188">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-188">Boolean</span></span>|<span data-ttu-id="71410-189">Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-190">applePayDisabled</span></span>|<span data-ttu-id="71410-191">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-191">Boolean</span></span>|<span data-ttu-id="71410-192">Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-193">zoomDisabled</span></span>|<span data-ttu-id="71410-194">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-194">Boolean</span></span>|<span data-ttu-id="71410-195">Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-196">siriDisabled</span></span>|<span data-ttu-id="71410-197">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-197">Boolean</span></span>|<span data-ttu-id="71410-198">Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-199">diagnosticsDisabled</span></span>|<span data-ttu-id="71410-200">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-200">Boolean</span></span>|<span data-ttu-id="71410-201">Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71410-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="71410-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-202">registrationDisabled</span></span>|<span data-ttu-id="71410-203">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-203">Boolean</span></span>|<span data-ttu-id="71410-204">Указывает, отключена при регистрации</span><span class="sxs-lookup"><span data-stu-id="71410-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="71410-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-205">fileVaultDisabled</span></span>|<span data-ttu-id="71410-206">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-206">Boolean</span></span>|<span data-ttu-id="71410-207">Указывает, если отключено хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="71410-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="71410-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="71410-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="71410-209">Логический</span><span class="sxs-lookup"><span data-stu-id="71410-209">Boolean</span></span>|<span data-ttu-id="71410-210">Указывает, если экран анализа iCloud отключен</span><span class="sxs-lookup"><span data-stu-id="71410-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="71410-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="71410-211">Response</span></span>
<span data-ttu-id="71410-212">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71410-212">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71410-213">Пример</span><span class="sxs-lookup"><span data-stu-id="71410-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="71410-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="71410-214">Request</span></span>
<span data-ttu-id="71410-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71410-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 928

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="71410-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="71410-216">Response</span></span>
<span data-ttu-id="71410-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="71410-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





