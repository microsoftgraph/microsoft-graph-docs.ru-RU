---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0b33d4c8ed70c5391d1bc5f85761dfac6f61a76
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941662"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="06da1-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="06da1-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="06da1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06da1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06da1-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06da1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06da1-107">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="06da1-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="06da1-108">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="06da1-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="06da1-109">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="06da1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="06da1-110">Methods</span></span>
|<span data-ttu-id="06da1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="06da1-111">Method</span></span>|<span data-ttu-id="06da1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="06da1-112">Return Type</span></span>|<span data-ttu-id="06da1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="06da1-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06da1-114">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="06da1-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="06da1-115">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="06da1-116">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="06da1-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="06da1-117">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="06da1-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="06da1-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="06da1-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="06da1-119">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="06da1-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06da1-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="06da1-120">Properties</span></span>
|<span data-ttu-id="06da1-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="06da1-121">Property</span></span>|<span data-ttu-id="06da1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="06da1-122">Type</span></span>|<span data-ttu-id="06da1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="06da1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06da1-124">id</span><span class="sxs-lookup"><span data-stu-id="06da1-124">id</span></span>|<span data-ttu-id="06da1-125">String</span><span class="sxs-lookup"><span data-stu-id="06da1-125">String</span></span>|<span data-ttu-id="06da1-126">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06da1-127">displayName</span><span class="sxs-lookup"><span data-stu-id="06da1-127">displayName</span></span>|<span data-ttu-id="06da1-128">Строка</span><span class="sxs-lookup"><span data-stu-id="06da1-128">String</span></span>|<span data-ttu-id="06da1-129">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06da1-130">description</span><span class="sxs-lookup"><span data-stu-id="06da1-130">description</span></span>|<span data-ttu-id="06da1-131">String</span><span class="sxs-lookup"><span data-stu-id="06da1-131">String</span></span>|<span data-ttu-id="06da1-132">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06da1-133">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="06da1-133">requiresUserAuthentication</span></span>|<span data-ttu-id="06da1-134">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-134">Boolean</span></span>|<span data-ttu-id="06da1-135">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06da1-136">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="06da1-136">configurationEndpointUrl</span></span>|<span data-ttu-id="06da1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="06da1-137">String</span></span>|<span data-ttu-id="06da1-138">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06da1-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="06da1-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="06da1-140">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-140">Boolean</span></span>|<span data-ttu-id="06da1-141">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="06da1-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="06da1-142">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06da1-143">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="06da1-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="06da1-144">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-144">Boolean</span></span>|<span data-ttu-id="06da1-145">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="06da1-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="06da1-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="06da1-146">isDefault</span></span>|<span data-ttu-id="06da1-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="06da1-147">Boolean</span></span>|<span data-ttu-id="06da1-148">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="06da1-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="06da1-149">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-149">supervisedModeEnabled</span></span>|<span data-ttu-id="06da1-150">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-150">Boolean</span></span>|<span data-ttu-id="06da1-151">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="06da1-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="06da1-152">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="06da1-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="06da1-153">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="06da1-153">supportDepartment</span></span>|<span data-ttu-id="06da1-154">Строка</span><span class="sxs-lookup"><span data-stu-id="06da1-154">String</span></span>|<span data-ttu-id="06da1-155">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="06da1-155">Support department information</span></span>|
|<span data-ttu-id="06da1-156">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-156">passCodeDisabled</span></span>|<span data-ttu-id="06da1-157">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-157">Boolean</span></span>|<span data-ttu-id="06da1-158">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="06da1-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-159">Обязательный</span><span class="sxs-lookup"><span data-stu-id="06da1-159">isMandatory</span></span>|<span data-ttu-id="06da1-160">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-160">Boolean</span></span>|<span data-ttu-id="06da1-161">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="06da1-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="06da1-162">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-162">locationDisabled</span></span>|<span data-ttu-id="06da1-163">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-163">Boolean</span></span>|<span data-ttu-id="06da1-164">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="06da1-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-165">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="06da1-165">supportPhoneNumber</span></span>|<span data-ttu-id="06da1-166">Строка</span><span class="sxs-lookup"><span data-stu-id="06da1-166">String</span></span>|<span data-ttu-id="06da1-167">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="06da1-167">Support phone number</span></span>|
|<span data-ttu-id="06da1-168">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-168">profileRemovalDisabled</span></span>|<span data-ttu-id="06da1-169">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-169">Boolean</span></span>|<span data-ttu-id="06da1-170">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="06da1-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="06da1-171">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="06da1-171">restoreBlocked</span></span>|<span data-ttu-id="06da1-172">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-172">Boolean</span></span>|<span data-ttu-id="06da1-173">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="06da1-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="06da1-174">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-174">appleIdDisabled</span></span>|<span data-ttu-id="06da1-175">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-175">Boolean</span></span>|<span data-ttu-id="06da1-176">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="06da1-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-177">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="06da1-178">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-178">Boolean</span></span>|<span data-ttu-id="06da1-179">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="06da1-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-180">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-180">touchIdDisabled</span></span>|<span data-ttu-id="06da1-181">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-181">Boolean</span></span>|<span data-ttu-id="06da1-182">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="06da1-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-183">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-183">applePayDisabled</span></span>|<span data-ttu-id="06da1-184">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-184">Boolean</span></span>|<span data-ttu-id="06da1-185">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="06da1-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-186">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-186">zoomDisabled</span></span>|<span data-ttu-id="06da1-187">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-187">Boolean</span></span>|<span data-ttu-id="06da1-188">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="06da1-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-189">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-189">siriDisabled</span></span>|<span data-ttu-id="06da1-190">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-190">Boolean</span></span>|<span data-ttu-id="06da1-191">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="06da1-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-192">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-192">diagnosticsDisabled</span></span>|<span data-ttu-id="06da1-193">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-193">Boolean</span></span>|<span data-ttu-id="06da1-194">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="06da1-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="06da1-195">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="06da1-196">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-196">Boolean</span></span>|<span data-ttu-id="06da1-197">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="06da1-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="06da1-198">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="06da1-198">privacyPaneDisabled</span></span>|<span data-ttu-id="06da1-199">Логический</span><span class="sxs-lookup"><span data-stu-id="06da1-199">Boolean</span></span>|<span data-ttu-id="06da1-200">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="06da1-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="06da1-201">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="06da1-201">deviceNameTemplate</span></span>|<span data-ttu-id="06da1-202">Строка</span><span class="sxs-lookup"><span data-stu-id="06da1-202">String</span></span>|<span data-ttu-id="06da1-203">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="06da1-203">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06da1-204">Связи</span><span class="sxs-lookup"><span data-stu-id="06da1-204">Relationships</span></span>
<span data-ttu-id="06da1-205">Нет</span><span class="sxs-lookup"><span data-stu-id="06da1-205">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06da1-206">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06da1-206">JSON Representation</span></span>
<span data-ttu-id="06da1-207">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06da1-207">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```




