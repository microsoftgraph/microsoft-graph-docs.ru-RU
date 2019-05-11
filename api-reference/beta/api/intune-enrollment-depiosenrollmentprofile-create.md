---
title: Создание Депиосенроллментпрофиле
description: Создание нового объекта Депиосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f18a1e8bba5446a505db7750aa7f238baba13fd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908933"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="a657c-103">Создание Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a657c-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="a657c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a657c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a657c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a657c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a657c-106">Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a657c-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a657c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a657c-107">Prerequisites</span></span>
<span data-ttu-id="a657c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a657c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a657c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a657c-110">Permission type</span></span>|<span data-ttu-id="a657c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a657c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a657c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a657c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a657c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a657c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a657c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a657c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a657c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a657c-115">Not supported.</span></span>|
|<span data-ttu-id="a657c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a657c-116">Application</span></span>|<span data-ttu-id="a657c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a657c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a657c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a657c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a657c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a657c-119">Request headers</span></span>
|<span data-ttu-id="a657c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a657c-120">Header</span></span>|<span data-ttu-id="a657c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a657c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a657c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a657c-122">Authorization</span></span>|<span data-ttu-id="a657c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a657c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a657c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a657c-124">Accept</span></span>|<span data-ttu-id="a657c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a657c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a657c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a657c-126">Request body</span></span>
<span data-ttu-id="a657c-127">В тексте запроса добавьте представление объекта Депиосенроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a657c-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="a657c-128">В следующей таблице приведены свойства, необходимые при создании Депиосенроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="a657c-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="a657c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a657c-129">Property</span></span>|<span data-ttu-id="a657c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a657c-130">Type</span></span>|<span data-ttu-id="a657c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a657c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a657c-132">id</span><span class="sxs-lookup"><span data-stu-id="a657c-132">id</span></span>|<span data-ttu-id="a657c-133">String</span><span class="sxs-lookup"><span data-stu-id="a657c-133">String</span></span>|<span data-ttu-id="a657c-134">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a657c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a657c-135">displayName</span></span>|<span data-ttu-id="a657c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a657c-136">String</span></span>|<span data-ttu-id="a657c-137">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a657c-138">description</span><span class="sxs-lookup"><span data-stu-id="a657c-138">description</span></span>|<span data-ttu-id="a657c-139">String</span><span class="sxs-lookup"><span data-stu-id="a657c-139">String</span></span>|<span data-ttu-id="a657c-140">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a657c-141">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="a657c-141">requiresUserAuthentication</span></span>|<span data-ttu-id="a657c-142">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-142">Boolean</span></span>|<span data-ttu-id="a657c-143">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a657c-144">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="a657c-144">configurationEndpointUrl</span></span>|<span data-ttu-id="a657c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="a657c-145">String</span></span>|<span data-ttu-id="a657c-146">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a657c-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="a657c-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="a657c-148">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-148">Boolean</span></span>|<span data-ttu-id="a657c-149">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="a657c-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="a657c-150">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a657c-151">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="a657c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="a657c-152">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-152">Boolean</span></span>|<span data-ttu-id="a657c-153">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a657c-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="a657c-154">isDefault</span></span>|<span data-ttu-id="a657c-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="a657c-155">Boolean</span></span>|<span data-ttu-id="a657c-156">Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-157">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-157">supervisedModeEnabled</span></span>|<span data-ttu-id="a657c-158">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-158">Boolean</span></span>|<span data-ttu-id="a657c-159">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="a657c-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="a657c-160">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="a657c-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="a657c-161">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-162">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="a657c-162">supportDepartment</span></span>|<span data-ttu-id="a657c-163">Строка</span><span class="sxs-lookup"><span data-stu-id="a657c-163">String</span></span>|<span data-ttu-id="a657c-164">Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-165">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-165">passCodeDisabled</span></span>|<span data-ttu-id="a657c-166">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-166">Boolean</span></span>|<span data-ttu-id="a657c-167">Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-168">Обязательный</span><span class="sxs-lookup"><span data-stu-id="a657c-168">isMandatory</span></span>|<span data-ttu-id="a657c-169">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-169">Boolean</span></span>|<span data-ttu-id="a657c-170">Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-171">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-171">locationDisabled</span></span>|<span data-ttu-id="a657c-172">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-172">Boolean</span></span>|<span data-ttu-id="a657c-173">Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-174">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="a657c-174">supportPhoneNumber</span></span>|<span data-ttu-id="a657c-175">Строка</span><span class="sxs-lookup"><span data-stu-id="a657c-175">String</span></span>|<span data-ttu-id="a657c-176">Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-177">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-177">profileRemovalDisabled</span></span>|<span data-ttu-id="a657c-178">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-178">Boolean</span></span>|<span data-ttu-id="a657c-179">Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-180">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="a657c-180">restoreBlocked</span></span>|<span data-ttu-id="a657c-181">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-181">Boolean</span></span>|<span data-ttu-id="a657c-182">Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-183">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-183">appleIdDisabled</span></span>|<span data-ttu-id="a657c-184">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-184">Boolean</span></span>|<span data-ttu-id="a657c-185">Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-186">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="a657c-187">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-187">Boolean</span></span>|<span data-ttu-id="a657c-188">Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-189">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-189">touchIdDisabled</span></span>|<span data-ttu-id="a657c-190">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-190">Boolean</span></span>|<span data-ttu-id="a657c-191">Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-192">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-192">applePayDisabled</span></span>|<span data-ttu-id="a657c-193">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-193">Boolean</span></span>|<span data-ttu-id="a657c-194">Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-195">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-195">zoomDisabled</span></span>|<span data-ttu-id="a657c-196">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-196">Boolean</span></span>|<span data-ttu-id="a657c-197">Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-198">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-198">siriDisabled</span></span>|<span data-ttu-id="a657c-199">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-199">Boolean</span></span>|<span data-ttu-id="a657c-200">Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-201">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-201">diagnosticsDisabled</span></span>|<span data-ttu-id="a657c-202">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-202">Boolean</span></span>|<span data-ttu-id="a657c-203">Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-204">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="a657c-205">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-205">Boolean</span></span>|<span data-ttu-id="a657c-206">Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-207">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-207">privacyPaneDisabled</span></span>|<span data-ttu-id="a657c-208">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-208">Boolean</span></span>|<span data-ttu-id="a657c-209">Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-210">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="a657c-210">deviceNameTemplate</span></span>|<span data-ttu-id="a657c-211">Строка</span><span class="sxs-lookup"><span data-stu-id="a657c-211">String</span></span>|<span data-ttu-id="a657c-212">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="a657c-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="a657c-213">Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a657c-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="a657c-214">iTunesPairingMode</span></span>|<span data-ttu-id="a657c-215">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).</span><span class="sxs-lookup"><span data-stu-id="a657c-215">[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)</span></span>|<span data-ttu-id="a657c-216">Указывает режим связывания iTunes.</span><span class="sxs-lookup"><span data-stu-id="a657c-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="a657c-217">Возможные значения: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="a657c-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="a657c-218">Манажементцертификатес</span><span class="sxs-lookup"><span data-stu-id="a657c-218">managementCertificates</span></span>|<span data-ttu-id="a657c-219">Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="a657c-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="a657c-220">Сертификаты управления для конфигуратора Apple</span><span class="sxs-lookup"><span data-stu-id="a657c-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="a657c-221">Ресторефромандроиддисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="a657c-222">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-222">Boolean</span></span>|<span data-ttu-id="a657c-223">Указывает, отключено ли восстановление из Android</span><span class="sxs-lookup"><span data-stu-id="a657c-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="a657c-224">Аваитдевицеконфигуредконфирматион</span><span class="sxs-lookup"><span data-stu-id="a657c-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="a657c-225">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-225">Boolean</span></span>|<span data-ttu-id="a657c-226">Указывает, должно ли устройство ждать настройки подтверждения.</span><span class="sxs-lookup"><span data-stu-id="a657c-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="a657c-227">Свойства sharedipadmaximumusercount</span><span class="sxs-lookup"><span data-stu-id="a657c-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="a657c-228">Int32</span><span class="sxs-lookup"><span data-stu-id="a657c-228">Int32</span></span>|<span data-ttu-id="a657c-229">Указывает максимальное количество пользователей, которые могут использовать общий iPad.</span><span class="sxs-lookup"><span data-stu-id="a657c-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="a657c-230">Относится только к общему режиму iPad.</span><span class="sxs-lookup"><span data-stu-id="a657c-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="a657c-231">Enablesharedipad к</span><span class="sxs-lookup"><span data-stu-id="a657c-231">enableSharedIPad</span></span>|<span data-ttu-id="a657c-232">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-232">Boolean</span></span>|<span data-ttu-id="a657c-233">Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями.</span><span class="sxs-lookup"><span data-stu-id="a657c-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="a657c-234">Применяется только в общих iPad.</span><span class="sxs-lookup"><span data-stu-id="a657c-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="a657c-235">Компанипорталвпптокенид</span><span class="sxs-lookup"><span data-stu-id="a657c-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="a657c-236">Строка</span><span class="sxs-lookup"><span data-stu-id="a657c-236">String</span></span>|<span data-ttu-id="a657c-237">Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство".</span><span class="sxs-lookup"><span data-stu-id="a657c-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="a657c-238">для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".</span><span class="sxs-lookup"><span data-stu-id="a657c-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="a657c-239">Енаблесинглеаппенроллментмоде</span><span class="sxs-lookup"><span data-stu-id="a657c-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="a657c-240">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-240">Boolean</span></span>|<span data-ttu-id="a657c-241">Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="a657c-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="a657c-242">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="a657c-242">Default is false.</span></span> <span data-ttu-id="a657c-243">для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".</span><span class="sxs-lookup"><span data-stu-id="a657c-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="a657c-244">Хомебуттонскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="a657c-245">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-245">Boolean</span></span>|<span data-ttu-id="a657c-246">Указывает, отключен ли экран "чувствительность к домашней кнопке"</span><span class="sxs-lookup"><span data-stu-id="a657c-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="a657c-247">Имессажеандфацетимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="a657c-248">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-248">Boolean</span></span>|<span data-ttu-id="a657c-249">Указывает, отключен ли экран iMessage и FaceTime</span><span class="sxs-lookup"><span data-stu-id="a657c-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="a657c-250">Онбоардингскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="a657c-251">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-251">Boolean</span></span>|<span data-ttu-id="a657c-252">Указывает, отключен ли встроенный экран установки</span><span class="sxs-lookup"><span data-stu-id="a657c-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="a657c-253">Скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="a657c-254">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-254">Boolean</span></span>|<span data-ttu-id="a657c-255">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="a657c-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="a657c-256">Симсетупскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="a657c-257">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-257">Boolean</span></span>|<span data-ttu-id="a657c-258">Указывает, отключен ли экран Симсетуп</span><span class="sxs-lookup"><span data-stu-id="a657c-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="a657c-259">Софтвареупдатескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="a657c-260">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-260">Boolean</span></span>|<span data-ttu-id="a657c-261">Указывает, отключено ли обязательное экранное обновление софваре</span><span class="sxs-lookup"><span data-stu-id="a657c-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="a657c-262">Ватчмигратионскриндисаблед</span><span class="sxs-lookup"><span data-stu-id="a657c-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="a657c-263">Логический</span><span class="sxs-lookup"><span data-stu-id="a657c-263">Boolean</span></span>|<span data-ttu-id="a657c-264">Указывает, отключен ли экран контрольных значений для миграции</span><span class="sxs-lookup"><span data-stu-id="a657c-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="a657c-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="a657c-265">Response</span></span>
<span data-ttu-id="a657c-266">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a657c-266">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a657c-267">Пример</span><span class="sxs-lookup"><span data-stu-id="a657c-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="a657c-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="a657c-268">Request</span></span>
<span data-ttu-id="a657c-269">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a657c-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1791

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
  "deviceNameTemplate": "Device Name Template value",
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

### <a name="response"></a><span data-ttu-id="a657c-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="a657c-270">Response</span></span>
<span data-ttu-id="a657c-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a657c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1840

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
  "deviceNameTemplate": "Device Name Template value",
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




