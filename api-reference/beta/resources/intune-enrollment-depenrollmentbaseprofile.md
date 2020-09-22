---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3878177d847cd4c98908345f8e1de66b22218bb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080350"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="d8a77-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="d8a77-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="d8a77-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8a77-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8a77-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a77-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8a77-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8a77-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8a77-108">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="d8a77-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="d8a77-109">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="d8a77-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="d8a77-110">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d8a77-111">Методы</span><span class="sxs-lookup"><span data-stu-id="d8a77-111">Methods</span></span>
|<span data-ttu-id="d8a77-112">Метод</span><span class="sxs-lookup"><span data-stu-id="d8a77-112">Method</span></span>|<span data-ttu-id="d8a77-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8a77-113">Return Type</span></span>|<span data-ttu-id="d8a77-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a77-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8a77-115">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="d8a77-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="d8a77-116">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="d8a77-117">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d8a77-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="d8a77-118">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="d8a77-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="d8a77-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="d8a77-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="d8a77-120">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d8a77-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8a77-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8a77-121">Properties</span></span>
|<span data-ttu-id="d8a77-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8a77-122">Property</span></span>|<span data-ttu-id="d8a77-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d8a77-123">Type</span></span>|<span data-ttu-id="d8a77-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a77-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8a77-125">id</span><span class="sxs-lookup"><span data-stu-id="d8a77-125">id</span></span>|<span data-ttu-id="d8a77-126">String</span><span class="sxs-lookup"><span data-stu-id="d8a77-126">String</span></span>|<span data-ttu-id="d8a77-127">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8a77-128">displayName</span><span class="sxs-lookup"><span data-stu-id="d8a77-128">displayName</span></span>|<span data-ttu-id="d8a77-129">String</span><span class="sxs-lookup"><span data-stu-id="d8a77-129">String</span></span>|<span data-ttu-id="d8a77-130">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8a77-131">description</span><span class="sxs-lookup"><span data-stu-id="d8a77-131">description</span></span>|<span data-ttu-id="d8a77-132">String</span><span class="sxs-lookup"><span data-stu-id="d8a77-132">String</span></span>|<span data-ttu-id="d8a77-133">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8a77-134">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="d8a77-134">requiresUserAuthentication</span></span>|<span data-ttu-id="d8a77-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-135">Boolean</span></span>|<span data-ttu-id="d8a77-136">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8a77-137">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="d8a77-137">configurationEndpointUrl</span></span>|<span data-ttu-id="d8a77-138">String</span><span class="sxs-lookup"><span data-stu-id="d8a77-138">String</span></span>|<span data-ttu-id="d8a77-139">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8a77-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d8a77-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d8a77-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-141">Boolean</span></span>|<span data-ttu-id="d8a77-142">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="d8a77-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d8a77-143">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8a77-144">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="d8a77-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d8a77-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-145">Boolean</span></span>|<span data-ttu-id="d8a77-146">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d8a77-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d8a77-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="d8a77-147">isDefault</span></span>|<span data-ttu-id="d8a77-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-148">Boolean</span></span>|<span data-ttu-id="d8a77-149">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d8a77-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="d8a77-150">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-150">supervisedModeEnabled</span></span>|<span data-ttu-id="d8a77-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-151">Boolean</span></span>|<span data-ttu-id="d8a77-152">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="d8a77-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d8a77-153">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="d8a77-153">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="d8a77-154">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="d8a77-154">supportDepartment</span></span>|<span data-ttu-id="d8a77-155">String</span><span class="sxs-lookup"><span data-stu-id="d8a77-155">String</span></span>|<span data-ttu-id="d8a77-156">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="d8a77-156">Support department information</span></span>|
|<span data-ttu-id="d8a77-157">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-157">passCodeDisabled</span></span>|<span data-ttu-id="d8a77-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-158">Boolean</span></span>|<span data-ttu-id="d8a77-159">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="d8a77-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-160">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d8a77-160">isMandatory</span></span>|<span data-ttu-id="d8a77-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-161">Boolean</span></span>|<span data-ttu-id="d8a77-162">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="d8a77-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="d8a77-163">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-163">locationDisabled</span></span>|<span data-ttu-id="d8a77-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-164">Boolean</span></span>|<span data-ttu-id="d8a77-165">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="d8a77-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-166">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="d8a77-166">supportPhoneNumber</span></span>|<span data-ttu-id="d8a77-167">String</span><span class="sxs-lookup"><span data-stu-id="d8a77-167">String</span></span>|<span data-ttu-id="d8a77-168">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="d8a77-168">Support phone number</span></span>|
|<span data-ttu-id="d8a77-169">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-169">profileRemovalDisabled</span></span>|<span data-ttu-id="d8a77-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-170">Boolean</span></span>|<span data-ttu-id="d8a77-171">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="d8a77-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="d8a77-172">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="d8a77-172">restoreBlocked</span></span>|<span data-ttu-id="d8a77-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-173">Boolean</span></span>|<span data-ttu-id="d8a77-174">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="d8a77-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="d8a77-175">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-175">appleIdDisabled</span></span>|<span data-ttu-id="d8a77-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-176">Boolean</span></span>|<span data-ttu-id="d8a77-177">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="d8a77-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-178">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d8a77-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-179">Boolean</span></span>|<span data-ttu-id="d8a77-180">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="d8a77-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-181">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-181">touchIdDisabled</span></span>|<span data-ttu-id="d8a77-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-182">Boolean</span></span>|<span data-ttu-id="d8a77-183">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="d8a77-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-184">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-184">applePayDisabled</span></span>|<span data-ttu-id="d8a77-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-185">Boolean</span></span>|<span data-ttu-id="d8a77-186">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="d8a77-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-187">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-187">zoomDisabled</span></span>|<span data-ttu-id="d8a77-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-188">Boolean</span></span>|<span data-ttu-id="d8a77-189">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="d8a77-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-190">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-190">siriDisabled</span></span>|<span data-ttu-id="d8a77-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-191">Boolean</span></span>|<span data-ttu-id="d8a77-192">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="d8a77-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-193">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-193">diagnosticsDisabled</span></span>|<span data-ttu-id="d8a77-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-194">Boolean</span></span>|<span data-ttu-id="d8a77-195">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="d8a77-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="d8a77-196">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="d8a77-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-197">Boolean</span></span>|<span data-ttu-id="d8a77-198">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="d8a77-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="d8a77-199">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-199">privacyPaneDisabled</span></span>|<span data-ttu-id="d8a77-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-200">Boolean</span></span>|<span data-ttu-id="d8a77-201">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="d8a77-201">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="d8a77-202">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="d8a77-202">screenTimeScreenDisabled</span></span>|<span data-ttu-id="d8a77-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-203">Boolean</span></span>|<span data-ttu-id="d8a77-204">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="d8a77-204">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="d8a77-205">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="d8a77-205">deviceNameTemplate</span></span>|<span data-ttu-id="d8a77-206">String</span><span class="sxs-lookup"><span data-stu-id="d8a77-206">String</span></span>|<span data-ttu-id="d8a77-207">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="d8a77-207">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="d8a77-208">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="d8a77-208">configurationWebUrl</span></span>|<span data-ttu-id="d8a77-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8a77-209">Boolean</span></span>|<span data-ttu-id="d8a77-210">URL-адрес для входа в помощнике по настройке</span><span class="sxs-lookup"><span data-stu-id="d8a77-210">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8a77-211">Отношения</span><span class="sxs-lookup"><span data-stu-id="d8a77-211">Relationships</span></span>
<span data-ttu-id="d8a77-212">Нет</span><span class="sxs-lookup"><span data-stu-id="d8a77-212">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8a77-213">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8a77-213">JSON Representation</span></span>
<span data-ttu-id="d8a77-214">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8a77-214">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "String",
  "configurationWebUrl": true
}
```






