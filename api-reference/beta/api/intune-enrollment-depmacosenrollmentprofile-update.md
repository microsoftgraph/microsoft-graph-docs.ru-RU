---
title: Обновление depMacOSEnrollmentProfile
description: Обновление свойства объекта depMacOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f86e520160e988e72aaa2473b256613a997cae0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420117"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="42a54-103">Обновление depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="42a54-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="42a54-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42a54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42a54-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42a54-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42a54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42a54-107">Обновление свойства объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="42a54-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42a54-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="42a54-108">Prerequisites</span></span>
<span data-ttu-id="42a54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42a54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42a54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42a54-111">Permission type</span></span>|<span data-ttu-id="42a54-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42a54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42a54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42a54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42a54-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42a54-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42a54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42a54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42a54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a54-116">Not supported.</span></span>|
|<span data-ttu-id="42a54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42a54-117">Application</span></span>|<span data-ttu-id="42a54-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42a54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42a54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42a54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="42a54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42a54-120">Request headers</span></span>
|<span data-ttu-id="42a54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42a54-121">Header</span></span>|<span data-ttu-id="42a54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42a54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42a54-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42a54-123">Authorization</span></span>|<span data-ttu-id="42a54-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42a54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42a54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42a54-125">Accept</span></span>|<span data-ttu-id="42a54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42a54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42a54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42a54-127">Request body</span></span>
<span data-ttu-id="42a54-128">В тексте запроса укажите представление JSON для объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="42a54-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="42a54-129">В следующей таблице показаны свойства, которые необходимы для создания [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="42a54-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="42a54-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42a54-130">Property</span></span>|<span data-ttu-id="42a54-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42a54-131">Type</span></span>|<span data-ttu-id="42a54-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42a54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42a54-133">id</span><span class="sxs-lookup"><span data-stu-id="42a54-133">id</span></span>|<span data-ttu-id="42a54-134">String</span><span class="sxs-lookup"><span data-stu-id="42a54-134">String</span></span>|<span data-ttu-id="42a54-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="42a54-136">displayName</span><span class="sxs-lookup"><span data-stu-id="42a54-136">displayName</span></span>|<span data-ttu-id="42a54-137">String</span><span class="sxs-lookup"><span data-stu-id="42a54-137">String</span></span>|<span data-ttu-id="42a54-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="42a54-139">description</span><span class="sxs-lookup"><span data-stu-id="42a54-139">description</span></span>|<span data-ttu-id="42a54-140">String</span><span class="sxs-lookup"><span data-stu-id="42a54-140">String</span></span>|<span data-ttu-id="42a54-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="42a54-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="42a54-142">requiresUserAuthentication</span></span>|<span data-ttu-id="42a54-143">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-143">Boolean</span></span>|<span data-ttu-id="42a54-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="42a54-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="42a54-145">configurationEndpointUrl</span></span>|<span data-ttu-id="42a54-146">String</span><span class="sxs-lookup"><span data-stu-id="42a54-146">String</span></span>|<span data-ttu-id="42a54-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="42a54-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="42a54-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="42a54-149">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-149">Boolean</span></span>|<span data-ttu-id="42a54-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="42a54-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="42a54-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="42a54-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="42a54-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="42a54-153">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-153">Boolean</span></span>|<span data-ttu-id="42a54-154">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="42a54-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="42a54-155">isDefault</span></span>|<span data-ttu-id="42a54-156">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-156">Boolean</span></span>|<span data-ttu-id="42a54-157">Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="42a54-158">supervisedModeEnabled</span></span>|<span data-ttu-id="42a54-159">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-159">Boolean</span></span>|<span data-ttu-id="42a54-160">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="42a54-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="42a54-161">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="42a54-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="42a54-162">Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="42a54-163">supportDepartment</span></span>|<span data-ttu-id="42a54-164">String</span><span class="sxs-lookup"><span data-stu-id="42a54-164">String</span></span>|<span data-ttu-id="42a54-165">Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-166">passCodeDisabled</span></span>|<span data-ttu-id="42a54-167">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-167">Boolean</span></span>|<span data-ttu-id="42a54-168">Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="42a54-169">isMandatory</span></span>|<span data-ttu-id="42a54-170">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-170">Boolean</span></span>|<span data-ttu-id="42a54-171">Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-172">locationDisabled</span></span>|<span data-ttu-id="42a54-173">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-173">Boolean</span></span>|<span data-ttu-id="42a54-174">Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="42a54-175">supportPhoneNumber</span></span>|<span data-ttu-id="42a54-176">String</span><span class="sxs-lookup"><span data-stu-id="42a54-176">String</span></span>|<span data-ttu-id="42a54-177">Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-178">profileRemovalDisabled</span></span>|<span data-ttu-id="42a54-179">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-179">Boolean</span></span>|<span data-ttu-id="42a54-180">Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="42a54-181">restoreBlocked</span></span>|<span data-ttu-id="42a54-182">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-182">Boolean</span></span>|<span data-ttu-id="42a54-183">Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-184">appleIdDisabled</span></span>|<span data-ttu-id="42a54-185">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-185">Boolean</span></span>|<span data-ttu-id="42a54-186">Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="42a54-188">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-188">Boolean</span></span>|<span data-ttu-id="42a54-189">Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-190">touchIdDisabled</span></span>|<span data-ttu-id="42a54-191">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-191">Boolean</span></span>|<span data-ttu-id="42a54-192">Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-193">applePayDisabled</span></span>|<span data-ttu-id="42a54-194">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-194">Boolean</span></span>|<span data-ttu-id="42a54-195">Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-196">zoomDisabled</span></span>|<span data-ttu-id="42a54-197">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-197">Boolean</span></span>|<span data-ttu-id="42a54-198">Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-199">siriDisabled</span></span>|<span data-ttu-id="42a54-200">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-200">Boolean</span></span>|<span data-ttu-id="42a54-201">Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-202">diagnosticsDisabled</span></span>|<span data-ttu-id="42a54-203">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-203">Boolean</span></span>|<span data-ttu-id="42a54-204">Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="42a54-206">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-206">Boolean</span></span>|<span data-ttu-id="42a54-207">Указывает, если экран установки displaytone отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-208">privacyPaneDisabled</span></span>|<span data-ttu-id="42a54-209">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-209">Boolean</span></span>|<span data-ttu-id="42a54-210">Указывает, если отключено экрана конфиденциальности наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42a54-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="42a54-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-211">registrationDisabled</span></span>|<span data-ttu-id="42a54-212">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-212">Boolean</span></span>|<span data-ttu-id="42a54-213">Указывает, отключена при регистрации</span><span class="sxs-lookup"><span data-stu-id="42a54-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="42a54-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-214">fileVaultDisabled</span></span>|<span data-ttu-id="42a54-215">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-215">Boolean</span></span>|<span data-ttu-id="42a54-216">Указывает, если отключено хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="42a54-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="42a54-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="42a54-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="42a54-218">Логический</span><span class="sxs-lookup"><span data-stu-id="42a54-218">Boolean</span></span>|<span data-ttu-id="42a54-219">Указывает, если экран анализа iCloud отключен</span><span class="sxs-lookup"><span data-stu-id="42a54-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="42a54-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a54-220">Response</span></span>
<span data-ttu-id="42a54-221">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42a54-221">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42a54-222">Пример</span><span class="sxs-lookup"><span data-stu-id="42a54-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="42a54-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="42a54-223">Request</span></span>
<span data-ttu-id="42a54-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42a54-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1061

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="42a54-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="42a54-225">Response</span></span>
<span data-ttu-id="42a54-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42a54-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```




