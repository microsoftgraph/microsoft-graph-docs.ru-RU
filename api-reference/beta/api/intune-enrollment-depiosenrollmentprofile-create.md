---
title: Создание depIOSEnrollmentProfile
description: Создание нового объекта depIOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 164cfeef009f63e3318c59f2428483c60673bd10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858032"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="b0052-103">Создание depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="b0052-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="b0052-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b0052-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0052-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0052-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0052-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b0052-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0052-107">Создание нового объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b0052-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0052-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b0052-108">Prerequisites</span></span>
<span data-ttu-id="b0052-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0052-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0052-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0052-111">Permission type</span></span>|<span data-ttu-id="b0052-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0052-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0052-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0052-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0052-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0052-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b0052-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0052-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0052-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0052-116">Not supported.</span></span>|
|<span data-ttu-id="b0052-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0052-117">Application</span></span>|<span data-ttu-id="b0052-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0052-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0052-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0052-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="b0052-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0052-120">Request headers</span></span>
|<span data-ttu-id="b0052-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0052-121">Header</span></span>|<span data-ttu-id="b0052-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b0052-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0052-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0052-123">Authorization</span></span>|<span data-ttu-id="b0052-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b0052-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0052-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0052-125">Accept</span></span>|<span data-ttu-id="b0052-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0052-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0052-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0052-127">Request body</span></span>
<span data-ttu-id="b0052-128">В тексте запроса укажите представление JSON для объекта depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="b0052-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="b0052-129">В следующей таблице показаны свойства, которые необходимы для создания depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="b0052-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="b0052-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0052-130">Property</span></span>|<span data-ttu-id="b0052-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b0052-131">Type</span></span>|<span data-ttu-id="b0052-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b0052-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0052-133">id</span><span class="sxs-lookup"><span data-stu-id="b0052-133">id</span></span>|<span data-ttu-id="b0052-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b0052-134">String</span></span>|<span data-ttu-id="b0052-135">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0052-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b0052-136">displayName</span></span>|<span data-ttu-id="b0052-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b0052-137">String</span></span>|<span data-ttu-id="b0052-138">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0052-139">описание</span><span class="sxs-lookup"><span data-stu-id="b0052-139">description</span></span>|<span data-ttu-id="b0052-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b0052-140">String</span></span>|<span data-ttu-id="b0052-141">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0052-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="b0052-142">requiresUserAuthentication</span></span>|<span data-ttu-id="b0052-143">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-143">Boolean</span></span>|<span data-ttu-id="b0052-144">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0052-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="b0052-145">configurationEndpointUrl</span></span>|<span data-ttu-id="b0052-146">Строка</span><span class="sxs-lookup"><span data-stu-id="b0052-146">String</span></span>|<span data-ttu-id="b0052-147">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0052-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="b0052-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="b0052-149">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-149">Boolean</span></span>|<span data-ttu-id="b0052-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="b0052-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="b0052-151">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="b0052-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="b0052-152">isDefault</span></span>|<span data-ttu-id="b0052-153">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-153">Boolean</span></span>|<span data-ttu-id="b0052-154">Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="b0052-155">supervisedModeEnabled</span></span>|<span data-ttu-id="b0052-156">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-156">Boolean</span></span>|<span data-ttu-id="b0052-157">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="b0052-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="b0052-158">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="b0052-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="b0052-159">Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="b0052-160">supportDepartment</span></span>|<span data-ttu-id="b0052-161">Строка</span><span class="sxs-lookup"><span data-stu-id="b0052-161">String</span></span>|<span data-ttu-id="b0052-162">Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-163">passCodeDisabled</span></span>|<span data-ttu-id="b0052-164">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-164">Boolean</span></span>|<span data-ttu-id="b0052-165">Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="b0052-166">isMandatory</span></span>|<span data-ttu-id="b0052-167">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-167">Boolean</span></span>|<span data-ttu-id="b0052-168">Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-169">locationDisabled</span></span>|<span data-ttu-id="b0052-170">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-170">Boolean</span></span>|<span data-ttu-id="b0052-171">Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b0052-172">supportPhoneNumber</span></span>|<span data-ttu-id="b0052-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b0052-173">String</span></span>|<span data-ttu-id="b0052-174">Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-175">profileRemovalDisabled</span></span>|<span data-ttu-id="b0052-176">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-176">Boolean</span></span>|<span data-ttu-id="b0052-177">Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b0052-178">restoreBlocked</span></span>|<span data-ttu-id="b0052-179">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-179">Boolean</span></span>|<span data-ttu-id="b0052-180">Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-181">appleIdDisabled</span></span>|<span data-ttu-id="b0052-182">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-182">Boolean</span></span>|<span data-ttu-id="b0052-183">Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="b0052-185">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-185">Boolean</span></span>|<span data-ttu-id="b0052-186">Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-187">touchIdDisabled</span></span>|<span data-ttu-id="b0052-188">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-188">Boolean</span></span>|<span data-ttu-id="b0052-189">Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-190">applePayDisabled</span></span>|<span data-ttu-id="b0052-191">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-191">Boolean</span></span>|<span data-ttu-id="b0052-192">Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-193">zoomDisabled</span></span>|<span data-ttu-id="b0052-194">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-194">Boolean</span></span>|<span data-ttu-id="b0052-195">Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-196">siriDisabled</span></span>|<span data-ttu-id="b0052-197">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-197">Boolean</span></span>|<span data-ttu-id="b0052-198">Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-199">diagnosticsDisabled</span></span>|<span data-ttu-id="b0052-200">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-200">Boolean</span></span>|<span data-ttu-id="b0052-201">Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b0052-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="b0052-202">iTunesPairingMode.</span><span class="sxs-lookup"><span data-stu-id="b0052-202">iTunesPairingMode</span></span>|<span data-ttu-id="b0052-203">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="b0052-203">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="b0052-204">Указывает iTunes, режим связывания.</span><span class="sxs-lookup"><span data-stu-id="b0052-204">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="b0052-205">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="b0052-205">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="b0052-206">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="b0052-206">managementCertificates</span></span>|<span data-ttu-id="b0052-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b0052-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="b0052-208">Управление сертификатами для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="b0052-208">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="b0052-209">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="b0052-209">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="b0052-210">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-210">Boolean</span></span>|<span data-ttu-id="b0052-211">Указывает, если отключено восстановление из Android (en)</span><span class="sxs-lookup"><span data-stu-id="b0052-211">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="b0052-212">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="b0052-212">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="b0052-213">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-213">Boolean</span></span>|<span data-ttu-id="b0052-214">Указывает, если устройство необходимо подождать настроенного подтверждения</span><span class="sxs-lookup"><span data-stu-id="b0052-214">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="b0052-215">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="b0052-215">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="b0052-216">Int32</span><span class="sxs-lookup"><span data-stu-id="b0052-216">Int32</span></span>|<span data-ttu-id="b0052-217">Это указывает максимальное количество пользователей, которые могут использовать общие iPad.</span><span class="sxs-lookup"><span data-stu-id="b0052-217">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="b0052-218">Применим только в режиме общего iPad.</span><span class="sxs-lookup"><span data-stu-id="b0052-218">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="b0052-219">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="b0052-219">enableSharedIPad</span></span>|<span data-ttu-id="b0052-220">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-220">Boolean</span></span>|<span data-ttu-id="b0052-221">Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии.</span><span class="sxs-lookup"><span data-stu-id="b0052-221">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="b0052-222">Применим только в общих iPads.</span><span class="sxs-lookup"><span data-stu-id="b0052-222">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="b0052-223">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="b0052-223">companyPortalVppTokenId</span></span>|<span data-ttu-id="b0052-224">Строка</span><span class="sxs-lookup"><span data-stu-id="b0052-224">String</span></span>|<span data-ttu-id="b0052-225">Если значение, указывает, какие Vpp маркер следует использовать для развертывания портала компании с устройства лицензирования.</span><span class="sxs-lookup"><span data-stu-id="b0052-225">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="b0052-226">«enableAuthenticationViaCompanyPortal» необходимо задать для этого свойства должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="b0052-226">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="b0052-227">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="b0052-227">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="b0052-228">Логический</span><span class="sxs-lookup"><span data-stu-id="b0052-228">Boolean</span></span>|<span data-ttu-id="b0052-229">Указывает устройство, чтобы включить режим одного приложения и применение блокировки приложения во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="b0052-229">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="b0052-230">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="b0052-230">Default is false.</span></span> <span data-ttu-id="b0052-231">«enableAuthenticationViaCompanyPortal» и «companyPortalVppTokenId» необходимо задать для этого свойства должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="b0052-231">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|



## <a name="response"></a><span data-ttu-id="b0052-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0052-232">Response</span></span>
<span data-ttu-id="b0052-233">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b0052-233">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0052-234">Пример</span><span class="sxs-lookup"><span data-stu-id="b0052-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0052-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0052-235">Request</span></span>
<span data-ttu-id="b0052-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0052-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1329

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "enableSingleAppEnrollmentMode": true
}
```

### <a name="response"></a><span data-ttu-id="b0052-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0052-237">Response</span></span>
<span data-ttu-id="b0052-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b0052-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1378

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
  "enableSingleAppEnrollmentMode": true
}
```





