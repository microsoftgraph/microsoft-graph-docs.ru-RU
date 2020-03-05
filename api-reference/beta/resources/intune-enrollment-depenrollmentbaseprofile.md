---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b3845b693dcc3030e8e24062d496b4c1fb19bcd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524768"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="72774-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="72774-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="72774-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72774-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72774-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72774-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72774-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72774-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72774-108">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="72774-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="72774-109">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="72774-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="72774-110">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="72774-111">Методы</span><span class="sxs-lookup"><span data-stu-id="72774-111">Methods</span></span>
|<span data-ttu-id="72774-112">Метод</span><span class="sxs-lookup"><span data-stu-id="72774-112">Method</span></span>|<span data-ttu-id="72774-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72774-113">Return Type</span></span>|<span data-ttu-id="72774-114">Описание</span><span class="sxs-lookup"><span data-stu-id="72774-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72774-115">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="72774-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="72774-116">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="72774-117">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="72774-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="72774-118">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="72774-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="72774-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="72774-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="72774-120">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="72774-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72774-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="72774-121">Properties</span></span>
|<span data-ttu-id="72774-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="72774-122">Property</span></span>|<span data-ttu-id="72774-123">Тип</span><span class="sxs-lookup"><span data-stu-id="72774-123">Type</span></span>|<span data-ttu-id="72774-124">Описание</span><span class="sxs-lookup"><span data-stu-id="72774-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72774-125">id</span><span class="sxs-lookup"><span data-stu-id="72774-125">id</span></span>|<span data-ttu-id="72774-126">String</span><span class="sxs-lookup"><span data-stu-id="72774-126">String</span></span>|<span data-ttu-id="72774-127">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="72774-128">displayName</span><span class="sxs-lookup"><span data-stu-id="72774-128">displayName</span></span>|<span data-ttu-id="72774-129">Строка</span><span class="sxs-lookup"><span data-stu-id="72774-129">String</span></span>|<span data-ttu-id="72774-130">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="72774-131">description</span><span class="sxs-lookup"><span data-stu-id="72774-131">description</span></span>|<span data-ttu-id="72774-132">String</span><span class="sxs-lookup"><span data-stu-id="72774-132">String</span></span>|<span data-ttu-id="72774-133">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="72774-134">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="72774-134">requiresUserAuthentication</span></span>|<span data-ttu-id="72774-135">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-135">Boolean</span></span>|<span data-ttu-id="72774-136">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="72774-137">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="72774-137">configurationEndpointUrl</span></span>|<span data-ttu-id="72774-138">String</span><span class="sxs-lookup"><span data-stu-id="72774-138">String</span></span>|<span data-ttu-id="72774-139">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="72774-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="72774-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="72774-141">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-141">Boolean</span></span>|<span data-ttu-id="72774-142">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="72774-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="72774-143">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="72774-144">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="72774-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="72774-145">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-145">Boolean</span></span>|<span data-ttu-id="72774-146">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="72774-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="72774-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="72774-147">isDefault</span></span>|<span data-ttu-id="72774-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="72774-148">Boolean</span></span>|<span data-ttu-id="72774-149">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="72774-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="72774-150">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="72774-150">supervisedModeEnabled</span></span>|<span data-ttu-id="72774-151">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-151">Boolean</span></span>|<span data-ttu-id="72774-152">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="72774-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="72774-153">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="72774-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="72774-154">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="72774-154">supportDepartment</span></span>|<span data-ttu-id="72774-155">String</span><span class="sxs-lookup"><span data-stu-id="72774-155">String</span></span>|<span data-ttu-id="72774-156">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="72774-156">Support department information</span></span>|
|<span data-ttu-id="72774-157">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-157">passCodeDisabled</span></span>|<span data-ttu-id="72774-158">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-158">Boolean</span></span>|<span data-ttu-id="72774-159">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="72774-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="72774-160">Обязательный</span><span class="sxs-lookup"><span data-stu-id="72774-160">isMandatory</span></span>|<span data-ttu-id="72774-161">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-161">Boolean</span></span>|<span data-ttu-id="72774-162">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="72774-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="72774-163">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-163">locationDisabled</span></span>|<span data-ttu-id="72774-164">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-164">Boolean</span></span>|<span data-ttu-id="72774-165">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="72774-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="72774-166">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="72774-166">supportPhoneNumber</span></span>|<span data-ttu-id="72774-167">String</span><span class="sxs-lookup"><span data-stu-id="72774-167">String</span></span>|<span data-ttu-id="72774-168">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="72774-168">Support phone number</span></span>|
|<span data-ttu-id="72774-169">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-169">profileRemovalDisabled</span></span>|<span data-ttu-id="72774-170">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-170">Boolean</span></span>|<span data-ttu-id="72774-171">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="72774-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="72774-172">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="72774-172">restoreBlocked</span></span>|<span data-ttu-id="72774-173">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-173">Boolean</span></span>|<span data-ttu-id="72774-174">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="72774-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="72774-175">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-175">appleIdDisabled</span></span>|<span data-ttu-id="72774-176">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-176">Boolean</span></span>|<span data-ttu-id="72774-177">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="72774-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="72774-178">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="72774-179">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-179">Boolean</span></span>|<span data-ttu-id="72774-180">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="72774-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="72774-181">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-181">touchIdDisabled</span></span>|<span data-ttu-id="72774-182">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-182">Boolean</span></span>|<span data-ttu-id="72774-183">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="72774-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="72774-184">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-184">applePayDisabled</span></span>|<span data-ttu-id="72774-185">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-185">Boolean</span></span>|<span data-ttu-id="72774-186">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="72774-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="72774-187">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-187">zoomDisabled</span></span>|<span data-ttu-id="72774-188">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-188">Boolean</span></span>|<span data-ttu-id="72774-189">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="72774-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="72774-190">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-190">siriDisabled</span></span>|<span data-ttu-id="72774-191">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-191">Boolean</span></span>|<span data-ttu-id="72774-192">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="72774-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="72774-193">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-193">diagnosticsDisabled</span></span>|<span data-ttu-id="72774-194">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-194">Boolean</span></span>|<span data-ttu-id="72774-195">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="72774-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="72774-196">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="72774-197">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-197">Boolean</span></span>|<span data-ttu-id="72774-198">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="72774-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="72774-199">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-199">privacyPaneDisabled</span></span>|<span data-ttu-id="72774-200">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-200">Boolean</span></span>|<span data-ttu-id="72774-201">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="72774-201">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="72774-202">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="72774-202">screenTimeScreenDisabled</span></span>|<span data-ttu-id="72774-203">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-203">Boolean</span></span>|<span data-ttu-id="72774-204">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="72774-204">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="72774-205">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="72774-205">deviceNameTemplate</span></span>|<span data-ttu-id="72774-206">String</span><span class="sxs-lookup"><span data-stu-id="72774-206">String</span></span>|<span data-ttu-id="72774-207">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="72774-207">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="72774-208">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="72774-208">configurationWebUrl</span></span>|<span data-ttu-id="72774-209">Логический</span><span class="sxs-lookup"><span data-stu-id="72774-209">Boolean</span></span>|<span data-ttu-id="72774-210">URL-адрес для входа в помощнике по настройке</span><span class="sxs-lookup"><span data-stu-id="72774-210">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="72774-211">Связи</span><span class="sxs-lookup"><span data-stu-id="72774-211">Relationships</span></span>
<span data-ttu-id="72774-212">Нет</span><span class="sxs-lookup"><span data-stu-id="72774-212">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72774-213">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72774-213">JSON Representation</span></span>
<span data-ttu-id="72774-214">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72774-214">Here is a JSON representation of the resource.</span></span>
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



