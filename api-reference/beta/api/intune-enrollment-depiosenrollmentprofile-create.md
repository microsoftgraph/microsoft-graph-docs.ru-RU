---
title: Создание depIOSEnrollmentProfile
description: Создание нового объекта depIOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a716e088dd9bcad19bc01a23f012f1a3cd5b3373
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398788"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="a3f26-103">Создание depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a3f26-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="a3f26-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3f26-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a3f26-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3f26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3f26-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3f26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3f26-107">Создание нового объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a3f26-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3f26-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a3f26-108">Prerequisites</span></span>
<span data-ttu-id="a3f26-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3f26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a3f26-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3f26-111">Permission type</span></span>|<span data-ttu-id="a3f26-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3f26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3f26-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3f26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3f26-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3f26-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a3f26-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3f26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3f26-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3f26-116">Not supported.</span></span>|
|<span data-ttu-id="a3f26-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3f26-117">Application</span></span>|<span data-ttu-id="a3f26-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3f26-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3f26-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3f26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a3f26-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3f26-120">Request headers</span></span>
|<span data-ttu-id="a3f26-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3f26-121">Header</span></span>|<span data-ttu-id="a3f26-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3f26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3f26-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3f26-123">Authorization</span></span>|<span data-ttu-id="a3f26-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3f26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3f26-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3f26-125">Accept</span></span>|<span data-ttu-id="a3f26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3f26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3f26-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3f26-127">Request body</span></span>
<span data-ttu-id="a3f26-128">В тексте запроса укажите представление JSON для объекта depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a3f26-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="a3f26-129">В следующей таблице показаны свойства, которые необходимы для создания depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a3f26-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="a3f26-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3f26-130">Property</span></span>|<span data-ttu-id="a3f26-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3f26-131">Type</span></span>|<span data-ttu-id="a3f26-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3f26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3f26-133">id</span><span class="sxs-lookup"><span data-stu-id="a3f26-133">id</span></span>|<span data-ttu-id="a3f26-134">String</span><span class="sxs-lookup"><span data-stu-id="a3f26-134">String</span></span>|<span data-ttu-id="a3f26-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a3f26-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a3f26-136">displayName</span></span>|<span data-ttu-id="a3f26-137">String</span><span class="sxs-lookup"><span data-stu-id="a3f26-137">String</span></span>|<span data-ttu-id="a3f26-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a3f26-139">description</span><span class="sxs-lookup"><span data-stu-id="a3f26-139">description</span></span>|<span data-ttu-id="a3f26-140">String</span><span class="sxs-lookup"><span data-stu-id="a3f26-140">String</span></span>|<span data-ttu-id="a3f26-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a3f26-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="a3f26-142">requiresUserAuthentication</span></span>|<span data-ttu-id="a3f26-143">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-143">Boolean</span></span>|<span data-ttu-id="a3f26-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a3f26-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="a3f26-145">configurationEndpointUrl</span></span>|<span data-ttu-id="a3f26-146">String</span><span class="sxs-lookup"><span data-stu-id="a3f26-146">String</span></span>|<span data-ttu-id="a3f26-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a3f26-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="a3f26-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="a3f26-149">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-149">Boolean</span></span>|<span data-ttu-id="a3f26-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="a3f26-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="a3f26-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a3f26-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="a3f26-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="a3f26-153">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-153">Boolean</span></span>|<span data-ttu-id="a3f26-154">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a3f26-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="a3f26-155">isDefault</span></span>|<span data-ttu-id="a3f26-156">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-156">Boolean</span></span>|<span data-ttu-id="a3f26-157">Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-158">supervisedModeEnabled</span></span>|<span data-ttu-id="a3f26-159">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-159">Boolean</span></span>|<span data-ttu-id="a3f26-160">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="a3f26-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="a3f26-161">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="a3f26-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="a3f26-162">Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="a3f26-163">supportDepartment</span></span>|<span data-ttu-id="a3f26-164">String</span><span class="sxs-lookup"><span data-stu-id="a3f26-164">String</span></span>|<span data-ttu-id="a3f26-165">Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-166">passCodeDisabled</span></span>|<span data-ttu-id="a3f26-167">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-167">Boolean</span></span>|<span data-ttu-id="a3f26-168">Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="a3f26-169">isMandatory</span></span>|<span data-ttu-id="a3f26-170">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-170">Boolean</span></span>|<span data-ttu-id="a3f26-171">Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-172">locationDisabled</span></span>|<span data-ttu-id="a3f26-173">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-173">Boolean</span></span>|<span data-ttu-id="a3f26-174">Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a3f26-175">supportPhoneNumber</span></span>|<span data-ttu-id="a3f26-176">String</span><span class="sxs-lookup"><span data-stu-id="a3f26-176">String</span></span>|<span data-ttu-id="a3f26-177">Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-178">profileRemovalDisabled</span></span>|<span data-ttu-id="a3f26-179">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-179">Boolean</span></span>|<span data-ttu-id="a3f26-180">Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a3f26-181">restoreBlocked</span></span>|<span data-ttu-id="a3f26-182">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-182">Boolean</span></span>|<span data-ttu-id="a3f26-183">Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-184">appleIdDisabled</span></span>|<span data-ttu-id="a3f26-185">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-185">Boolean</span></span>|<span data-ttu-id="a3f26-186">Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="a3f26-188">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-188">Boolean</span></span>|<span data-ttu-id="a3f26-189">Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-190">touchIdDisabled</span></span>|<span data-ttu-id="a3f26-191">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-191">Boolean</span></span>|<span data-ttu-id="a3f26-192">Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-193">applePayDisabled</span></span>|<span data-ttu-id="a3f26-194">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-194">Boolean</span></span>|<span data-ttu-id="a3f26-195">Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-196">zoomDisabled</span></span>|<span data-ttu-id="a3f26-197">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-197">Boolean</span></span>|<span data-ttu-id="a3f26-198">Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-199">siriDisabled</span></span>|<span data-ttu-id="a3f26-200">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-200">Boolean</span></span>|<span data-ttu-id="a3f26-201">Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-202">diagnosticsDisabled</span></span>|<span data-ttu-id="a3f26-203">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-203">Boolean</span></span>|<span data-ttu-id="a3f26-204">Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="a3f26-206">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-206">Boolean</span></span>|<span data-ttu-id="a3f26-207">Указывает, если экран установки displaytone отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-208">privacyPaneDisabled</span></span>|<span data-ttu-id="a3f26-209">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-209">Boolean</span></span>|<span data-ttu-id="a3f26-210">Указывает, если отключено экрана конфиденциальности наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a3f26-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a3f26-211">iTunesPairingMode.</span><span class="sxs-lookup"><span data-stu-id="a3f26-211">iTunesPairingMode</span></span>|<span data-ttu-id="a3f26-212">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="a3f26-212">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="a3f26-213">Указывает iTunes, режим связывания.</span><span class="sxs-lookup"><span data-stu-id="a3f26-213">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="a3f26-214">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="a3f26-214">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="a3f26-215">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="a3f26-215">managementCertificates</span></span>|<span data-ttu-id="a3f26-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a3f26-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="a3f26-217">Управление сертификатами для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="a3f26-217">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="a3f26-218">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-218">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="a3f26-219">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-219">Boolean</span></span>|<span data-ttu-id="a3f26-220">Указывает, если отключено восстановление из Android (en)</span><span class="sxs-lookup"><span data-stu-id="a3f26-220">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="a3f26-221">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="a3f26-221">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="a3f26-222">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-222">Boolean</span></span>|<span data-ttu-id="a3f26-223">Указывает, если устройство необходимо подождать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="a3f26-223">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="a3f26-224">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="a3f26-224">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="a3f26-225">Int32</span><span class="sxs-lookup"><span data-stu-id="a3f26-225">Int32</span></span>|<span data-ttu-id="a3f26-226">Это указывает максимальное количество пользователей, которые могут использовать общие iPad.</span><span class="sxs-lookup"><span data-stu-id="a3f26-226">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="a3f26-227">Применим только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="a3f26-227">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="a3f26-228">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="a3f26-228">enableSharedIPad</span></span>|<span data-ttu-id="a3f26-229">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-229">Boolean</span></span>|<span data-ttu-id="a3f26-230">Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии.</span><span class="sxs-lookup"><span data-stu-id="a3f26-230">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="a3f26-231">Применим только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="a3f26-231">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="a3f26-232">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="a3f26-232">companyPortalVppTokenId</span></span>|<span data-ttu-id="a3f26-233">String</span><span class="sxs-lookup"><span data-stu-id="a3f26-233">String</span></span>|<span data-ttu-id="a3f26-234">Если значение, указывает, какие Vpp маркер следует использовать для развертывания портала компании с устройства лицензирования.</span><span class="sxs-lookup"><span data-stu-id="a3f26-234">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="a3f26-235">«enableAuthenticationViaCompanyPortal» необходимо задать для этого свойства должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="a3f26-235">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="a3f26-236">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="a3f26-236">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="a3f26-237">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-237">Boolean</span></span>|<span data-ttu-id="a3f26-238">Указывает устройство, чтобы включить режим одного приложения и применение блокировки приложения во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="a3f26-238">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="a3f26-239">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="a3f26-239">Default is false.</span></span> <span data-ttu-id="a3f26-240">«enableAuthenticationViaCompanyPortal» и «companyPortalVppTokenId» необходимо задать для этого свойства должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="a3f26-240">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="a3f26-241">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-241">homeButtonScreenDisabled</span></span>|<span data-ttu-id="a3f26-242">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-242">Boolean</span></span>|<span data-ttu-id="a3f26-243">Указывает, если уровень конфиденциальности сообщения окна кнопки Домой отключено</span><span class="sxs-lookup"><span data-stu-id="a3f26-243">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="a3f26-244">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-244">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="a3f26-245">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-245">Boolean</span></span>|<span data-ttu-id="a3f26-246">Указывает, если iMessage отключена FaceTime экрана</span><span class="sxs-lookup"><span data-stu-id="a3f26-246">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="a3f26-247">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-247">onBoardingScreenDisabled</span></span>|<span data-ttu-id="a3f26-248">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-248">Boolean</span></span>|<span data-ttu-id="a3f26-249">Указывает, если экран установки входящая отключен</span><span class="sxs-lookup"><span data-stu-id="a3f26-249">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="a3f26-250">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-250">screenTimeScreenDisabled</span></span>|<span data-ttu-id="a3f26-251">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-251">Boolean</span></span>|<span data-ttu-id="a3f26-252">Указывает, если экран установки времени ожидания отключен</span><span class="sxs-lookup"><span data-stu-id="a3f26-252">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="a3f26-253">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-253">simSetupScreenDisabled</span></span>|<span data-ttu-id="a3f26-254">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-254">Boolean</span></span>|<span data-ttu-id="a3f26-255">Указывает, если на экране SIMSetup отключен</span><span class="sxs-lookup"><span data-stu-id="a3f26-255">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="a3f26-256">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-256">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="a3f26-257">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-257">Boolean</span></span>|<span data-ttu-id="a3f26-258">Указывает, если на экране обязательные программа обновления отключен</span><span class="sxs-lookup"><span data-stu-id="a3f26-258">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="a3f26-259">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a3f26-259">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="a3f26-260">Логический</span><span class="sxs-lookup"><span data-stu-id="a3f26-260">Boolean</span></span>|<span data-ttu-id="a3f26-261">Указывает, если на экране миграции Контрольное значение отключено</span><span class="sxs-lookup"><span data-stu-id="a3f26-261">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="a3f26-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3f26-262">Response</span></span>
<span data-ttu-id="a3f26-263">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a3f26-263">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3f26-264">Пример</span><span class="sxs-lookup"><span data-stu-id="a3f26-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3f26-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3f26-265">Request</span></span>
<span data-ttu-id="a3f26-266">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3f26-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1736

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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="a3f26-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3f26-267">Response</span></span>
<span data-ttu-id="a3f26-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a3f26-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1785

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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




