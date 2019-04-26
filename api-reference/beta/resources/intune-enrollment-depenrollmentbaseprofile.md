---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69f0bb3647e5d12d0d441f06e7436626b0d29334
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573916"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="748ad-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="748ad-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="748ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="748ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="748ad-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="748ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="748ad-107">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="748ad-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="748ad-108">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="748ad-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="748ad-109">НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="748ad-110">Методы</span><span class="sxs-lookup"><span data-stu-id="748ad-110">Methods</span></span>
|<span data-ttu-id="748ad-111">Метод</span><span class="sxs-lookup"><span data-stu-id="748ad-111">Method</span></span>|<span data-ttu-id="748ad-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="748ad-112">Return Type</span></span>|<span data-ttu-id="748ad-113">Описание</span><span class="sxs-lookup"><span data-stu-id="748ad-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="748ad-114">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="748ad-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="748ad-115">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="748ad-116">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="748ad-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="748ad-117">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="748ad-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="748ad-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="748ad-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="748ad-119">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="748ad-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="748ad-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="748ad-120">Properties</span></span>
|<span data-ttu-id="748ad-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="748ad-121">Property</span></span>|<span data-ttu-id="748ad-122">Тип</span><span class="sxs-lookup"><span data-stu-id="748ad-122">Type</span></span>|<span data-ttu-id="748ad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="748ad-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="748ad-124">id</span><span class="sxs-lookup"><span data-stu-id="748ad-124">id</span></span>|<span data-ttu-id="748ad-125">Строка</span><span class="sxs-lookup"><span data-stu-id="748ad-125">String</span></span>|<span data-ttu-id="748ad-126">GUID объекта, наСледуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="748ad-127">displayName</span><span class="sxs-lookup"><span data-stu-id="748ad-127">displayName</span></span>|<span data-ttu-id="748ad-128">String</span><span class="sxs-lookup"><span data-stu-id="748ad-128">String</span></span>|<span data-ttu-id="748ad-129">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="748ad-130">description</span><span class="sxs-lookup"><span data-stu-id="748ad-130">description</span></span>|<span data-ttu-id="748ad-131">String</span><span class="sxs-lookup"><span data-stu-id="748ad-131">String</span></span>|<span data-ttu-id="748ad-132">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="748ad-133">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="748ad-133">requiresUserAuthentication</span></span>|<span data-ttu-id="748ad-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-134">Boolean</span></span>|<span data-ttu-id="748ad-135">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="748ad-136">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="748ad-136">configurationEndpointUrl</span></span>|<span data-ttu-id="748ad-137">String</span><span class="sxs-lookup"><span data-stu-id="748ad-137">String</span></span>|<span data-ttu-id="748ad-138">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="748ad-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="748ad-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="748ad-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-140">Boolean</span></span>|<span data-ttu-id="748ad-141">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="748ad-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="748ad-142">НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="748ad-143">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="748ad-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="748ad-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-144">Boolean</span></span>|<span data-ttu-id="748ad-145">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наСледуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="748ad-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="748ad-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="748ad-146">isDefault</span></span>|<span data-ttu-id="748ad-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-147">Boolean</span></span>|<span data-ttu-id="748ad-148">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="748ad-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="748ad-149">Супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-149">supervisedModeEnabled</span></span>|<span data-ttu-id="748ad-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-150">Boolean</span></span>|<span data-ttu-id="748ad-151">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="748ad-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="748ad-152">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="748ad-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="748ad-153">Суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="748ad-153">supportDepartment</span></span>|<span data-ttu-id="748ad-154">String</span><span class="sxs-lookup"><span data-stu-id="748ad-154">String</span></span>|<span data-ttu-id="748ad-155">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="748ad-155">Support department information</span></span>|
|<span data-ttu-id="748ad-156">Пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-156">passCodeDisabled</span></span>|<span data-ttu-id="748ad-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-157">Boolean</span></span>|<span data-ttu-id="748ad-158">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="748ad-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-159">Обязательный</span><span class="sxs-lookup"><span data-stu-id="748ad-159">isMandatory</span></span>|<span data-ttu-id="748ad-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-160">Boolean</span></span>|<span data-ttu-id="748ad-161">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="748ad-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="748ad-162">Локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-162">locationDisabled</span></span>|<span data-ttu-id="748ad-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-163">Boolean</span></span>|<span data-ttu-id="748ad-164">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="748ad-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-165">Суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="748ad-165">supportPhoneNumber</span></span>|<span data-ttu-id="748ad-166">String</span><span class="sxs-lookup"><span data-stu-id="748ad-166">String</span></span>|<span data-ttu-id="748ad-167">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="748ad-167">Support phone number</span></span>|
|<span data-ttu-id="748ad-168">Профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-168">profileRemovalDisabled</span></span>|<span data-ttu-id="748ad-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-169">Boolean</span></span>|<span data-ttu-id="748ad-170">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="748ad-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="748ad-171">Рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="748ad-171">restoreBlocked</span></span>|<span data-ttu-id="748ad-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-172">Boolean</span></span>|<span data-ttu-id="748ad-173">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="748ad-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="748ad-174">Апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-174">appleIdDisabled</span></span>|<span data-ttu-id="748ad-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-175">Boolean</span></span>|<span data-ttu-id="748ad-176">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="748ad-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-177">Термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="748ad-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-178">Boolean</span></span>|<span data-ttu-id="748ad-179">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="748ad-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-180">Таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-180">touchIdDisabled</span></span>|<span data-ttu-id="748ad-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-181">Boolean</span></span>|<span data-ttu-id="748ad-182">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="748ad-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-183">Апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-183">applePayDisabled</span></span>|<span data-ttu-id="748ad-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-184">Boolean</span></span>|<span data-ttu-id="748ad-185">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="748ad-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-186">Зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-186">zoomDisabled</span></span>|<span data-ttu-id="748ad-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-187">Boolean</span></span>|<span data-ttu-id="748ad-188">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="748ad-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-189">Сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-189">siriDisabled</span></span>|<span data-ttu-id="748ad-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-190">Boolean</span></span>|<span data-ttu-id="748ad-191">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="748ad-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-192">Диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-192">diagnosticsDisabled</span></span>|<span data-ttu-id="748ad-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-193">Boolean</span></span>|<span data-ttu-id="748ad-194">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="748ad-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="748ad-195">Дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="748ad-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-196">Boolean</span></span>|<span data-ttu-id="748ad-197">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="748ad-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="748ad-198">Приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="748ad-198">privacyPaneDisabled</span></span>|<span data-ttu-id="748ad-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="748ad-199">Boolean</span></span>|<span data-ttu-id="748ad-200">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="748ad-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="748ad-201">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="748ad-201">deviceNameTemplate</span></span>|<span data-ttu-id="748ad-202">String</span><span class="sxs-lookup"><span data-stu-id="748ad-202">String</span></span>|<span data-ttu-id="748ad-203">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="748ad-203">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="748ad-204">Отношения</span><span class="sxs-lookup"><span data-stu-id="748ad-204">Relationships</span></span>
<span data-ttu-id="748ad-205">Нет</span><span class="sxs-lookup"><span data-stu-id="748ad-205">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="748ad-206">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="748ad-206">JSON Representation</span></span>
<span data-ttu-id="748ad-207">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="748ad-207">Here is a JSON representation of the resource.</span></span>
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





