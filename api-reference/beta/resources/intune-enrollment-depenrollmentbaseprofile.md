---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed24aabc0f19ee6f9554a6d594c3095dcd4e3729
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207437"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="2afc3-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="2afc3-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="2afc3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2afc3-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2afc3-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2afc3-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2afc3-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2afc3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2afc3-108">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="2afc3-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="2afc3-109">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="2afc3-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="2afc3-110">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2afc3-111">Методы</span><span class="sxs-lookup"><span data-stu-id="2afc3-111">Methods</span></span>
|<span data-ttu-id="2afc3-112">Метод</span><span class="sxs-lookup"><span data-stu-id="2afc3-112">Method</span></span>|<span data-ttu-id="2afc3-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2afc3-113">Return Type</span></span>|<span data-ttu-id="2afc3-114">Описание</span><span class="sxs-lookup"><span data-stu-id="2afc3-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2afc3-115">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="2afc3-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="2afc3-116">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="2afc3-117">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2afc3-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="2afc3-118">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="2afc3-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="2afc3-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="2afc3-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="2afc3-120">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2afc3-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2afc3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="2afc3-121">Properties</span></span>
|<span data-ttu-id="2afc3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="2afc3-122">Property</span></span>|<span data-ttu-id="2afc3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2afc3-123">Type</span></span>|<span data-ttu-id="2afc3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2afc3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2afc3-125">id</span><span class="sxs-lookup"><span data-stu-id="2afc3-125">id</span></span>|<span data-ttu-id="2afc3-126">String</span><span class="sxs-lookup"><span data-stu-id="2afc3-126">String</span></span>|<span data-ttu-id="2afc3-127">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2afc3-128">displayName</span><span class="sxs-lookup"><span data-stu-id="2afc3-128">displayName</span></span>|<span data-ttu-id="2afc3-129">String</span><span class="sxs-lookup"><span data-stu-id="2afc3-129">String</span></span>|<span data-ttu-id="2afc3-130">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2afc3-131">description</span><span class="sxs-lookup"><span data-stu-id="2afc3-131">description</span></span>|<span data-ttu-id="2afc3-132">String</span><span class="sxs-lookup"><span data-stu-id="2afc3-132">String</span></span>|<span data-ttu-id="2afc3-133">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2afc3-134">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="2afc3-134">requiresUserAuthentication</span></span>|<span data-ttu-id="2afc3-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-135">Boolean</span></span>|<span data-ttu-id="2afc3-136">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2afc3-137">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="2afc3-137">configurationEndpointUrl</span></span>|<span data-ttu-id="2afc3-138">String</span><span class="sxs-lookup"><span data-stu-id="2afc3-138">String</span></span>|<span data-ttu-id="2afc3-139">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2afc3-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2afc3-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="2afc3-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-141">Boolean</span></span>|<span data-ttu-id="2afc3-142">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="2afc3-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="2afc3-143">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2afc3-144">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="2afc3-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="2afc3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-145">Boolean</span></span>|<span data-ttu-id="2afc3-146">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2afc3-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2afc3-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="2afc3-147">isDefault</span></span>|<span data-ttu-id="2afc3-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-148">Boolean</span></span>|<span data-ttu-id="2afc3-149">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="2afc3-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="2afc3-150">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-150">supervisedModeEnabled</span></span>|<span data-ttu-id="2afc3-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-151">Boolean</span></span>|<span data-ttu-id="2afc3-152">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="2afc3-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="2afc3-153"> https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="2afc3-153">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="2afc3-154">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="2afc3-154">supportDepartment</span></span>|<span data-ttu-id="2afc3-155">String</span><span class="sxs-lookup"><span data-stu-id="2afc3-155">String</span></span>|<span data-ttu-id="2afc3-156">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="2afc3-156">Support department information</span></span>|
|<span data-ttu-id="2afc3-157">Обязательный</span><span class="sxs-lookup"><span data-stu-id="2afc3-157">isMandatory</span></span>|<span data-ttu-id="2afc3-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-158">Boolean</span></span>|<span data-ttu-id="2afc3-159">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="2afc3-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="2afc3-160">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-160">locationDisabled</span></span>|<span data-ttu-id="2afc3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-161">Boolean</span></span>|<span data-ttu-id="2afc3-162">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="2afc3-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="2afc3-163">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="2afc3-163">supportPhoneNumber</span></span>|<span data-ttu-id="2afc3-164">String</span><span class="sxs-lookup"><span data-stu-id="2afc3-164">String</span></span>|<span data-ttu-id="2afc3-165">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="2afc3-165">Support phone number</span></span>|
|<span data-ttu-id="2afc3-166">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-166">profileRemovalDisabled</span></span>|<span data-ttu-id="2afc3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-167">Boolean</span></span>|<span data-ttu-id="2afc3-168">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="2afc3-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="2afc3-169">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="2afc3-169">restoreBlocked</span></span>|<span data-ttu-id="2afc3-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-170">Boolean</span></span>|<span data-ttu-id="2afc3-171">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="2afc3-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="2afc3-172">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-172">appleIdDisabled</span></span>|<span data-ttu-id="2afc3-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-173">Boolean</span></span>|<span data-ttu-id="2afc3-174">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="2afc3-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="2afc3-175">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="2afc3-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-176">Boolean</span></span>|<span data-ttu-id="2afc3-177">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="2afc3-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="2afc3-178">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-178">touchIdDisabled</span></span>|<span data-ttu-id="2afc3-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-179">Boolean</span></span>|<span data-ttu-id="2afc3-180">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="2afc3-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="2afc3-181">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-181">applePayDisabled</span></span>|<span data-ttu-id="2afc3-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-182">Boolean</span></span>|<span data-ttu-id="2afc3-183">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="2afc3-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="2afc3-184">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-184">siriDisabled</span></span>|<span data-ttu-id="2afc3-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-185">Boolean</span></span>|<span data-ttu-id="2afc3-186">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="2afc3-186">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="2afc3-187">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-187">diagnosticsDisabled</span></span>|<span data-ttu-id="2afc3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-188">Boolean</span></span>|<span data-ttu-id="2afc3-189">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="2afc3-189">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="2afc3-190">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-190">displayToneSetupDisabled</span></span>|<span data-ttu-id="2afc3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-191">Boolean</span></span>|<span data-ttu-id="2afc3-192">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="2afc3-192">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="2afc3-193">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-193">privacyPaneDisabled</span></span>|<span data-ttu-id="2afc3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-194">Boolean</span></span>|<span data-ttu-id="2afc3-195">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="2afc3-195">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="2afc3-196">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="2afc3-196">screenTimeScreenDisabled</span></span>|<span data-ttu-id="2afc3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-197">Boolean</span></span>|<span data-ttu-id="2afc3-198">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="2afc3-198">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="2afc3-199">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="2afc3-199">deviceNameTemplate</span></span>|<span data-ttu-id="2afc3-200">String</span><span class="sxs-lookup"><span data-stu-id="2afc3-200">String</span></span>|<span data-ttu-id="2afc3-201">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="2afc3-201">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="2afc3-202">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="2afc3-202">configurationWebUrl</span></span>|<span data-ttu-id="2afc3-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="2afc3-203">Boolean</span></span>|<span data-ttu-id="2afc3-204">URL-адрес для входа в помощнике по настройке</span><span class="sxs-lookup"><span data-stu-id="2afc3-204">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="2afc3-205">Связи</span><span class="sxs-lookup"><span data-stu-id="2afc3-205">Relationships</span></span>
<span data-ttu-id="2afc3-206">Нет</span><span class="sxs-lookup"><span data-stu-id="2afc3-206">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2afc3-207">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2afc3-207">JSON Representation</span></span>
<span data-ttu-id="2afc3-208">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2afc3-208">Here is a JSON representation of the resource.</span></span>
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




