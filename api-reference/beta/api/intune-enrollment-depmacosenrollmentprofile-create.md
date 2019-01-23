---
title: Создание depMacOSEnrollmentProfile
description: Создание нового объекта depMacOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7fd29ee598507b982ecd48ea58b6a09ccf90972
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420593"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="44d7c-103">Создание depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="44d7c-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="44d7c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44d7c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="44d7c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44d7c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44d7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44d7c-107">Создание нового объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="44d7c-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44d7c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="44d7c-108">Prerequisites</span></span>
<span data-ttu-id="44d7c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="44d7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44d7c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44d7c-111">Permission type</span></span>|<span data-ttu-id="44d7c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44d7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44d7c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44d7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44d7c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d7c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="44d7c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44d7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44d7c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d7c-116">Not supported.</span></span>|
|<span data-ttu-id="44d7c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44d7c-117">Application</span></span>|<span data-ttu-id="44d7c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d7c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44d7c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44d7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="44d7c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44d7c-120">Request headers</span></span>
|<span data-ttu-id="44d7c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44d7c-121">Header</span></span>|<span data-ttu-id="44d7c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44d7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44d7c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44d7c-123">Authorization</span></span>|<span data-ttu-id="44d7c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="44d7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44d7c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44d7c-125">Accept</span></span>|<span data-ttu-id="44d7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44d7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44d7c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44d7c-127">Request body</span></span>
<span data-ttu-id="44d7c-128">В тексте запроса укажите представление JSON для объекта depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="44d7c-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="44d7c-129">В следующей таблице показаны свойства, которые необходимы для создания depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="44d7c-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="44d7c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44d7c-130">Property</span></span>|<span data-ttu-id="44d7c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44d7c-131">Type</span></span>|<span data-ttu-id="44d7c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44d7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d7c-133">id</span><span class="sxs-lookup"><span data-stu-id="44d7c-133">id</span></span>|<span data-ttu-id="44d7c-134">String</span><span class="sxs-lookup"><span data-stu-id="44d7c-134">String</span></span>|<span data-ttu-id="44d7c-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="44d7c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="44d7c-136">displayName</span></span>|<span data-ttu-id="44d7c-137">String</span><span class="sxs-lookup"><span data-stu-id="44d7c-137">String</span></span>|<span data-ttu-id="44d7c-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="44d7c-139">description</span><span class="sxs-lookup"><span data-stu-id="44d7c-139">description</span></span>|<span data-ttu-id="44d7c-140">String</span><span class="sxs-lookup"><span data-stu-id="44d7c-140">String</span></span>|<span data-ttu-id="44d7c-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="44d7c-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="44d7c-142">requiresUserAuthentication</span></span>|<span data-ttu-id="44d7c-143">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-143">Boolean</span></span>|<span data-ttu-id="44d7c-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="44d7c-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="44d7c-145">configurationEndpointUrl</span></span>|<span data-ttu-id="44d7c-146">String</span><span class="sxs-lookup"><span data-stu-id="44d7c-146">String</span></span>|<span data-ttu-id="44d7c-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="44d7c-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="44d7c-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="44d7c-149">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-149">Boolean</span></span>|<span data-ttu-id="44d7c-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="44d7c-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="44d7c-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="44d7c-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="44d7c-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="44d7c-153">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-153">Boolean</span></span>|<span data-ttu-id="44d7c-154">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="44d7c-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="44d7c-155">isDefault</span></span>|<span data-ttu-id="44d7c-156">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-156">Boolean</span></span>|<span data-ttu-id="44d7c-157">Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-158">supervisedModeEnabled</span></span>|<span data-ttu-id="44d7c-159">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-159">Boolean</span></span>|<span data-ttu-id="44d7c-160">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="44d7c-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="44d7c-161">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="44d7c-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="44d7c-162">Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="44d7c-163">supportDepartment</span></span>|<span data-ttu-id="44d7c-164">String</span><span class="sxs-lookup"><span data-stu-id="44d7c-164">String</span></span>|<span data-ttu-id="44d7c-165">Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-166">passCodeDisabled</span></span>|<span data-ttu-id="44d7c-167">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-167">Boolean</span></span>|<span data-ttu-id="44d7c-168">Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="44d7c-169">isMandatory</span></span>|<span data-ttu-id="44d7c-170">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-170">Boolean</span></span>|<span data-ttu-id="44d7c-171">Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-172">locationDisabled</span></span>|<span data-ttu-id="44d7c-173">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-173">Boolean</span></span>|<span data-ttu-id="44d7c-174">Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="44d7c-175">supportPhoneNumber</span></span>|<span data-ttu-id="44d7c-176">String</span><span class="sxs-lookup"><span data-stu-id="44d7c-176">String</span></span>|<span data-ttu-id="44d7c-177">Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-178">profileRemovalDisabled</span></span>|<span data-ttu-id="44d7c-179">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-179">Boolean</span></span>|<span data-ttu-id="44d7c-180">Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="44d7c-181">restoreBlocked</span></span>|<span data-ttu-id="44d7c-182">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-182">Boolean</span></span>|<span data-ttu-id="44d7c-183">Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-184">appleIdDisabled</span></span>|<span data-ttu-id="44d7c-185">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-185">Boolean</span></span>|<span data-ttu-id="44d7c-186">Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="44d7c-188">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-188">Boolean</span></span>|<span data-ttu-id="44d7c-189">Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-190">touchIdDisabled</span></span>|<span data-ttu-id="44d7c-191">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-191">Boolean</span></span>|<span data-ttu-id="44d7c-192">Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-193">applePayDisabled</span></span>|<span data-ttu-id="44d7c-194">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-194">Boolean</span></span>|<span data-ttu-id="44d7c-195">Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-196">zoomDisabled</span></span>|<span data-ttu-id="44d7c-197">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-197">Boolean</span></span>|<span data-ttu-id="44d7c-198">Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-199">siriDisabled</span></span>|<span data-ttu-id="44d7c-200">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-200">Boolean</span></span>|<span data-ttu-id="44d7c-201">Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-202">diagnosticsDisabled</span></span>|<span data-ttu-id="44d7c-203">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-203">Boolean</span></span>|<span data-ttu-id="44d7c-204">Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="44d7c-206">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-206">Boolean</span></span>|<span data-ttu-id="44d7c-207">Указывает, если экран установки displaytone отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-208">privacyPaneDisabled</span></span>|<span data-ttu-id="44d7c-209">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-209">Boolean</span></span>|<span data-ttu-id="44d7c-210">Указывает, если отключено экрана конфиденциальности наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="44d7c-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="44d7c-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-211">registrationDisabled</span></span>|<span data-ttu-id="44d7c-212">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-212">Boolean</span></span>|<span data-ttu-id="44d7c-213">Указывает, отключена при регистрации</span><span class="sxs-lookup"><span data-stu-id="44d7c-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="44d7c-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-214">fileVaultDisabled</span></span>|<span data-ttu-id="44d7c-215">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-215">Boolean</span></span>|<span data-ttu-id="44d7c-216">Указывает, если отключено хранилище файлов</span><span class="sxs-lookup"><span data-stu-id="44d7c-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="44d7c-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="44d7c-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="44d7c-218">Логический</span><span class="sxs-lookup"><span data-stu-id="44d7c-218">Boolean</span></span>|<span data-ttu-id="44d7c-219">Указывает, если экран анализа iCloud отключен</span><span class="sxs-lookup"><span data-stu-id="44d7c-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="44d7c-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d7c-220">Response</span></span>
<span data-ttu-id="44d7c-221">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="44d7c-221">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44d7c-222">Пример</span><span class="sxs-lookup"><span data-stu-id="44d7c-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="44d7c-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d7c-223">Request</span></span>
<span data-ttu-id="44d7c-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d7c-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="44d7c-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d7c-225">Response</span></span>
<span data-ttu-id="44d7c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="44d7c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




