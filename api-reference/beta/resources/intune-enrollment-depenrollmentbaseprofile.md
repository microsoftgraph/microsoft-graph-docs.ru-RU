---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3bffd69ad5ce9c1a413504509c718afd0ce10e3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735234"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="0f493-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="0f493-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="0f493-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f493-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f493-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f493-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f493-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f493-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f493-108">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="0f493-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="0f493-109">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="0f493-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="0f493-110">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0f493-111">Методы</span><span class="sxs-lookup"><span data-stu-id="0f493-111">Methods</span></span>
|<span data-ttu-id="0f493-112">Метод</span><span class="sxs-lookup"><span data-stu-id="0f493-112">Method</span></span>|<span data-ttu-id="0f493-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f493-113">Return Type</span></span>|<span data-ttu-id="0f493-114">Описание</span><span class="sxs-lookup"><span data-stu-id="0f493-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f493-115">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="0f493-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="0f493-116">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="0f493-117">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0f493-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="0f493-118">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="0f493-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="0f493-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="0f493-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="0f493-120">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0f493-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f493-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f493-121">Properties</span></span>
|<span data-ttu-id="0f493-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f493-122">Property</span></span>|<span data-ttu-id="0f493-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0f493-123">Type</span></span>|<span data-ttu-id="0f493-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0f493-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f493-125">id</span><span class="sxs-lookup"><span data-stu-id="0f493-125">id</span></span>|<span data-ttu-id="0f493-126">Строка</span><span class="sxs-lookup"><span data-stu-id="0f493-126">String</span></span>|<span data-ttu-id="0f493-127">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0f493-128">displayName</span><span class="sxs-lookup"><span data-stu-id="0f493-128">displayName</span></span>|<span data-ttu-id="0f493-129">Строка</span><span class="sxs-lookup"><span data-stu-id="0f493-129">String</span></span>|<span data-ttu-id="0f493-130">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0f493-131">description</span><span class="sxs-lookup"><span data-stu-id="0f493-131">description</span></span>|<span data-ttu-id="0f493-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0f493-132">String</span></span>|<span data-ttu-id="0f493-133">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0f493-134">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="0f493-134">requiresUserAuthentication</span></span>|<span data-ttu-id="0f493-135">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-135">Boolean</span></span>|<span data-ttu-id="0f493-136">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0f493-137">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="0f493-137">configurationEndpointUrl</span></span>|<span data-ttu-id="0f493-138">Строка</span><span class="sxs-lookup"><span data-stu-id="0f493-138">String</span></span>|<span data-ttu-id="0f493-139">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0f493-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="0f493-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="0f493-141">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-141">Boolean</span></span>|<span data-ttu-id="0f493-142">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="0f493-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="0f493-143">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0f493-144">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="0f493-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="0f493-145">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-145">Boolean</span></span>|<span data-ttu-id="0f493-146">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f493-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0f493-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="0f493-147">isDefault</span></span>|<span data-ttu-id="0f493-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f493-148">Boolean</span></span>|<span data-ttu-id="0f493-149">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="0f493-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="0f493-150">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-150">supervisedModeEnabled</span></span>|<span data-ttu-id="0f493-151">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-151">Boolean</span></span>|<span data-ttu-id="0f493-152">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="0f493-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="0f493-153">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="0f493-153">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="0f493-154">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="0f493-154">supportDepartment</span></span>|<span data-ttu-id="0f493-155">Строка</span><span class="sxs-lookup"><span data-stu-id="0f493-155">String</span></span>|<span data-ttu-id="0f493-156">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="0f493-156">Support department information</span></span>|
|<span data-ttu-id="0f493-157">Обязательный</span><span class="sxs-lookup"><span data-stu-id="0f493-157">isMandatory</span></span>|<span data-ttu-id="0f493-158">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-158">Boolean</span></span>|<span data-ttu-id="0f493-159">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="0f493-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="0f493-160">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-160">locationDisabled</span></span>|<span data-ttu-id="0f493-161">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-161">Boolean</span></span>|<span data-ttu-id="0f493-162">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="0f493-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="0f493-163">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="0f493-163">supportPhoneNumber</span></span>|<span data-ttu-id="0f493-164">Строка</span><span class="sxs-lookup"><span data-stu-id="0f493-164">String</span></span>|<span data-ttu-id="0f493-165">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="0f493-165">Support phone number</span></span>|
|<span data-ttu-id="0f493-166">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-166">profileRemovalDisabled</span></span>|<span data-ttu-id="0f493-167">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-167">Boolean</span></span>|<span data-ttu-id="0f493-168">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="0f493-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="0f493-169">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="0f493-169">restoreBlocked</span></span>|<span data-ttu-id="0f493-170">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-170">Boolean</span></span>|<span data-ttu-id="0f493-171">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="0f493-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="0f493-172">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-172">appleIdDisabled</span></span>|<span data-ttu-id="0f493-173">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-173">Boolean</span></span>|<span data-ttu-id="0f493-174">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="0f493-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="0f493-175">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="0f493-176">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-176">Boolean</span></span>|<span data-ttu-id="0f493-177">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="0f493-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="0f493-178">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-178">touchIdDisabled</span></span>|<span data-ttu-id="0f493-179">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-179">Boolean</span></span>|<span data-ttu-id="0f493-180">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="0f493-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="0f493-181">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-181">applePayDisabled</span></span>|<span data-ttu-id="0f493-182">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-182">Boolean</span></span>|<span data-ttu-id="0f493-183">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="0f493-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="0f493-184">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-184">siriDisabled</span></span>|<span data-ttu-id="0f493-185">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-185">Boolean</span></span>|<span data-ttu-id="0f493-186">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="0f493-186">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="0f493-187">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-187">diagnosticsDisabled</span></span>|<span data-ttu-id="0f493-188">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-188">Boolean</span></span>|<span data-ttu-id="0f493-189">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="0f493-189">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="0f493-190">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-190">displayToneSetupDisabled</span></span>|<span data-ttu-id="0f493-191">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-191">Boolean</span></span>|<span data-ttu-id="0f493-192">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="0f493-192">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="0f493-193">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-193">privacyPaneDisabled</span></span>|<span data-ttu-id="0f493-194">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-194">Boolean</span></span>|<span data-ttu-id="0f493-195">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="0f493-195">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="0f493-196">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="0f493-196">screenTimeScreenDisabled</span></span>|<span data-ttu-id="0f493-197">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-197">Boolean</span></span>|<span data-ttu-id="0f493-198">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="0f493-198">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="0f493-199">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="0f493-199">deviceNameTemplate</span></span>|<span data-ttu-id="0f493-200">Строка</span><span class="sxs-lookup"><span data-stu-id="0f493-200">String</span></span>|<span data-ttu-id="0f493-201">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="0f493-201">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="0f493-202">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="0f493-202">configurationWebUrl</span></span>|<span data-ttu-id="0f493-203">Логический</span><span class="sxs-lookup"><span data-stu-id="0f493-203">Boolean</span></span>|<span data-ttu-id="0f493-204">URL-адрес для входа в помощнике по настройке</span><span class="sxs-lookup"><span data-stu-id="0f493-204">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f493-205">Связи</span><span class="sxs-lookup"><span data-stu-id="0f493-205">Relationships</span></span>
<span data-ttu-id="0f493-206">Нет</span><span class="sxs-lookup"><span data-stu-id="0f493-206">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f493-207">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f493-207">JSON Representation</span></span>
<span data-ttu-id="0f493-208">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f493-208">Here is a JSON representation of the resource.</span></span>
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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "String",
  "configurationWebUrl": true
}
```





