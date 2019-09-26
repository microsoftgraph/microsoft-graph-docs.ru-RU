---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0698380f3fb69323275a8c2db3725ddb741f2151
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196618"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="92f42-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="92f42-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="92f42-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92f42-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92f42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92f42-107">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="92f42-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="92f42-108">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="92f42-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="92f42-109">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="92f42-110">Методы</span><span class="sxs-lookup"><span data-stu-id="92f42-110">Methods</span></span>
|<span data-ttu-id="92f42-111">Метод</span><span class="sxs-lookup"><span data-stu-id="92f42-111">Method</span></span>|<span data-ttu-id="92f42-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92f42-112">Return Type</span></span>|<span data-ttu-id="92f42-113">Описание</span><span class="sxs-lookup"><span data-stu-id="92f42-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92f42-114">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="92f42-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="92f42-115">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="92f42-116">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="92f42-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="92f42-117">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="92f42-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="92f42-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="92f42-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="92f42-119">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="92f42-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="92f42-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="92f42-120">Properties</span></span>
|<span data-ttu-id="92f42-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="92f42-121">Property</span></span>|<span data-ttu-id="92f42-122">Тип</span><span class="sxs-lookup"><span data-stu-id="92f42-122">Type</span></span>|<span data-ttu-id="92f42-123">Описание</span><span class="sxs-lookup"><span data-stu-id="92f42-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92f42-124">id</span><span class="sxs-lookup"><span data-stu-id="92f42-124">id</span></span>|<span data-ttu-id="92f42-125">String</span><span class="sxs-lookup"><span data-stu-id="92f42-125">String</span></span>|<span data-ttu-id="92f42-126">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92f42-127">displayName</span><span class="sxs-lookup"><span data-stu-id="92f42-127">displayName</span></span>|<span data-ttu-id="92f42-128">Строка</span><span class="sxs-lookup"><span data-stu-id="92f42-128">String</span></span>|<span data-ttu-id="92f42-129">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92f42-130">description</span><span class="sxs-lookup"><span data-stu-id="92f42-130">description</span></span>|<span data-ttu-id="92f42-131">String</span><span class="sxs-lookup"><span data-stu-id="92f42-131">String</span></span>|<span data-ttu-id="92f42-132">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92f42-133">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="92f42-133">requiresUserAuthentication</span></span>|<span data-ttu-id="92f42-134">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-134">Boolean</span></span>|<span data-ttu-id="92f42-135">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92f42-136">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="92f42-136">configurationEndpointUrl</span></span>|<span data-ttu-id="92f42-137">String.</span><span class="sxs-lookup"><span data-stu-id="92f42-137">String</span></span>|<span data-ttu-id="92f42-138">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92f42-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="92f42-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="92f42-140">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-140">Boolean</span></span>|<span data-ttu-id="92f42-141">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="92f42-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="92f42-142">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92f42-143">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="92f42-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="92f42-144">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-144">Boolean</span></span>|<span data-ttu-id="92f42-145">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92f42-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="92f42-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="92f42-146">isDefault</span></span>|<span data-ttu-id="92f42-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="92f42-147">Boolean</span></span>|<span data-ttu-id="92f42-148">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="92f42-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="92f42-149">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-149">supervisedModeEnabled</span></span>|<span data-ttu-id="92f42-150">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-150">Boolean</span></span>|<span data-ttu-id="92f42-151">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="92f42-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="92f42-152">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="92f42-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="92f42-153">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="92f42-153">supportDepartment</span></span>|<span data-ttu-id="92f42-154">String.</span><span class="sxs-lookup"><span data-stu-id="92f42-154">String</span></span>|<span data-ttu-id="92f42-155">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="92f42-155">Support department information</span></span>|
|<span data-ttu-id="92f42-156">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-156">passCodeDisabled</span></span>|<span data-ttu-id="92f42-157">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-157">Boolean</span></span>|<span data-ttu-id="92f42-158">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="92f42-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-159">Обязательный</span><span class="sxs-lookup"><span data-stu-id="92f42-159">isMandatory</span></span>|<span data-ttu-id="92f42-160">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-160">Boolean</span></span>|<span data-ttu-id="92f42-161">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="92f42-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="92f42-162">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-162">locationDisabled</span></span>|<span data-ttu-id="92f42-163">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-163">Boolean</span></span>|<span data-ttu-id="92f42-164">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="92f42-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-165">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="92f42-165">supportPhoneNumber</span></span>|<span data-ttu-id="92f42-166">String.</span><span class="sxs-lookup"><span data-stu-id="92f42-166">String</span></span>|<span data-ttu-id="92f42-167">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="92f42-167">Support phone number</span></span>|
|<span data-ttu-id="92f42-168">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-168">profileRemovalDisabled</span></span>|<span data-ttu-id="92f42-169">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-169">Boolean</span></span>|<span data-ttu-id="92f42-170">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="92f42-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="92f42-171">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="92f42-171">restoreBlocked</span></span>|<span data-ttu-id="92f42-172">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-172">Boolean</span></span>|<span data-ttu-id="92f42-173">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="92f42-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="92f42-174">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-174">appleIdDisabled</span></span>|<span data-ttu-id="92f42-175">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-175">Boolean</span></span>|<span data-ttu-id="92f42-176">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="92f42-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-177">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="92f42-178">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-178">Boolean</span></span>|<span data-ttu-id="92f42-179">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="92f42-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-180">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-180">touchIdDisabled</span></span>|<span data-ttu-id="92f42-181">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-181">Boolean</span></span>|<span data-ttu-id="92f42-182">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="92f42-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-183">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-183">applePayDisabled</span></span>|<span data-ttu-id="92f42-184">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-184">Boolean</span></span>|<span data-ttu-id="92f42-185">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="92f42-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-186">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-186">zoomDisabled</span></span>|<span data-ttu-id="92f42-187">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-187">Boolean</span></span>|<span data-ttu-id="92f42-188">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="92f42-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-189">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-189">siriDisabled</span></span>|<span data-ttu-id="92f42-190">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-190">Boolean</span></span>|<span data-ttu-id="92f42-191">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="92f42-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-192">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-192">diagnosticsDisabled</span></span>|<span data-ttu-id="92f42-193">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-193">Boolean</span></span>|<span data-ttu-id="92f42-194">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="92f42-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="92f42-195">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="92f42-196">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-196">Boolean</span></span>|<span data-ttu-id="92f42-197">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="92f42-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="92f42-198">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-198">privacyPaneDisabled</span></span>|<span data-ttu-id="92f42-199">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-199">Boolean</span></span>|<span data-ttu-id="92f42-200">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="92f42-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="92f42-201">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="92f42-201">screenTimeScreenDisabled</span></span>|<span data-ttu-id="92f42-202">Boolean.</span><span class="sxs-lookup"><span data-stu-id="92f42-202">Boolean</span></span>|<span data-ttu-id="92f42-203">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="92f42-203">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="92f42-204">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="92f42-204">deviceNameTemplate</span></span>|<span data-ttu-id="92f42-205">String.</span><span class="sxs-lookup"><span data-stu-id="92f42-205">String</span></span>|<span data-ttu-id="92f42-206">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="92f42-206">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92f42-207">Отношения</span><span class="sxs-lookup"><span data-stu-id="92f42-207">Relationships</span></span>
<span data-ttu-id="92f42-208">Нет</span><span class="sxs-lookup"><span data-stu-id="92f42-208">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92f42-209">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92f42-209">JSON Representation</span></span>
<span data-ttu-id="92f42-210">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92f42-210">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```



