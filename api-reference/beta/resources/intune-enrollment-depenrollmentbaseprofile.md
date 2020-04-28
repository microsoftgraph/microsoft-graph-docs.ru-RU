---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ca200b9212f979660956a866e5a70ad47f4599a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358851"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="c0680-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="c0680-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="c0680-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0680-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0680-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0680-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0680-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0680-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0680-108">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="c0680-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="c0680-109">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="c0680-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="c0680-110">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c0680-111">Методы</span><span class="sxs-lookup"><span data-stu-id="c0680-111">Methods</span></span>
|<span data-ttu-id="c0680-112">Метод</span><span class="sxs-lookup"><span data-stu-id="c0680-112">Method</span></span>|<span data-ttu-id="c0680-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0680-113">Return Type</span></span>|<span data-ttu-id="c0680-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c0680-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0680-115">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="c0680-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="c0680-116">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="c0680-117">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c0680-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="c0680-118">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="c0680-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="c0680-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="c0680-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="c0680-120">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c0680-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0680-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0680-121">Properties</span></span>
|<span data-ttu-id="c0680-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0680-122">Property</span></span>|<span data-ttu-id="c0680-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c0680-123">Type</span></span>|<span data-ttu-id="c0680-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c0680-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0680-125">id</span><span class="sxs-lookup"><span data-stu-id="c0680-125">id</span></span>|<span data-ttu-id="c0680-126">String</span><span class="sxs-lookup"><span data-stu-id="c0680-126">String</span></span>|<span data-ttu-id="c0680-127">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c0680-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c0680-128">displayName</span></span>|<span data-ttu-id="c0680-129">Строка</span><span class="sxs-lookup"><span data-stu-id="c0680-129">String</span></span>|<span data-ttu-id="c0680-130">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c0680-131">description</span><span class="sxs-lookup"><span data-stu-id="c0680-131">description</span></span>|<span data-ttu-id="c0680-132">String</span><span class="sxs-lookup"><span data-stu-id="c0680-132">String</span></span>|<span data-ttu-id="c0680-133">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c0680-134">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="c0680-134">requiresUserAuthentication</span></span>|<span data-ttu-id="c0680-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-135">Boolean</span></span>|<span data-ttu-id="c0680-136">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c0680-137">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="c0680-137">configurationEndpointUrl</span></span>|<span data-ttu-id="c0680-138">String</span><span class="sxs-lookup"><span data-stu-id="c0680-138">String</span></span>|<span data-ttu-id="c0680-139">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c0680-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c0680-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c0680-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-141">Boolean</span></span>|<span data-ttu-id="c0680-142">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="c0680-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="c0680-143">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c0680-144">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="c0680-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="c0680-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-145">Boolean</span></span>|<span data-ttu-id="c0680-146">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c0680-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c0680-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="c0680-147">isDefault</span></span>|<span data-ttu-id="c0680-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-148">Boolean</span></span>|<span data-ttu-id="c0680-149">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="c0680-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="c0680-150">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-150">supervisedModeEnabled</span></span>|<span data-ttu-id="c0680-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-151">Boolean</span></span>|<span data-ttu-id="c0680-152">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="c0680-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="c0680-153">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="c0680-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="c0680-154">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="c0680-154">supportDepartment</span></span>|<span data-ttu-id="c0680-155">String</span><span class="sxs-lookup"><span data-stu-id="c0680-155">String</span></span>|<span data-ttu-id="c0680-156">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="c0680-156">Support department information</span></span>|
|<span data-ttu-id="c0680-157">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-157">passCodeDisabled</span></span>|<span data-ttu-id="c0680-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-158">Boolean</span></span>|<span data-ttu-id="c0680-159">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="c0680-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-160">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c0680-160">isMandatory</span></span>|<span data-ttu-id="c0680-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-161">Boolean</span></span>|<span data-ttu-id="c0680-162">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="c0680-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="c0680-163">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-163">locationDisabled</span></span>|<span data-ttu-id="c0680-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-164">Boolean</span></span>|<span data-ttu-id="c0680-165">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="c0680-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-166">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="c0680-166">supportPhoneNumber</span></span>|<span data-ttu-id="c0680-167">String</span><span class="sxs-lookup"><span data-stu-id="c0680-167">String</span></span>|<span data-ttu-id="c0680-168">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="c0680-168">Support phone number</span></span>|
|<span data-ttu-id="c0680-169">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-169">profileRemovalDisabled</span></span>|<span data-ttu-id="c0680-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-170">Boolean</span></span>|<span data-ttu-id="c0680-171">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="c0680-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="c0680-172">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="c0680-172">restoreBlocked</span></span>|<span data-ttu-id="c0680-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-173">Boolean</span></span>|<span data-ttu-id="c0680-174">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="c0680-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="c0680-175">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-175">appleIdDisabled</span></span>|<span data-ttu-id="c0680-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-176">Boolean</span></span>|<span data-ttu-id="c0680-177">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="c0680-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-178">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="c0680-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-179">Boolean</span></span>|<span data-ttu-id="c0680-180">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="c0680-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-181">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-181">touchIdDisabled</span></span>|<span data-ttu-id="c0680-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-182">Boolean</span></span>|<span data-ttu-id="c0680-183">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="c0680-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-184">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-184">applePayDisabled</span></span>|<span data-ttu-id="c0680-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-185">Boolean</span></span>|<span data-ttu-id="c0680-186">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="c0680-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-187">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-187">zoomDisabled</span></span>|<span data-ttu-id="c0680-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-188">Boolean</span></span>|<span data-ttu-id="c0680-189">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="c0680-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-190">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-190">siriDisabled</span></span>|<span data-ttu-id="c0680-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-191">Boolean</span></span>|<span data-ttu-id="c0680-192">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="c0680-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-193">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-193">diagnosticsDisabled</span></span>|<span data-ttu-id="c0680-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-194">Boolean</span></span>|<span data-ttu-id="c0680-195">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="c0680-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="c0680-196">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="c0680-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-197">Boolean</span></span>|<span data-ttu-id="c0680-198">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="c0680-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="c0680-199">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-199">privacyPaneDisabled</span></span>|<span data-ttu-id="c0680-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-200">Boolean</span></span>|<span data-ttu-id="c0680-201">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="c0680-201">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="c0680-202">скринтимескриндисаблед</span><span class="sxs-lookup"><span data-stu-id="c0680-202">screenTimeScreenDisabled</span></span>|<span data-ttu-id="c0680-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-203">Boolean</span></span>|<span data-ttu-id="c0680-204">Указывает, отключена ли настройка времени ожидания экрана</span><span class="sxs-lookup"><span data-stu-id="c0680-204">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="c0680-205">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="c0680-205">deviceNameTemplate</span></span>|<span data-ttu-id="c0680-206">String</span><span class="sxs-lookup"><span data-stu-id="c0680-206">String</span></span>|<span data-ttu-id="c0680-207">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="c0680-207">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="c0680-208">конфигуратионвебурл</span><span class="sxs-lookup"><span data-stu-id="c0680-208">configurationWebUrl</span></span>|<span data-ttu-id="c0680-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0680-209">Boolean</span></span>|<span data-ttu-id="c0680-210">URL-адрес для входа в помощнике по настройке</span><span class="sxs-lookup"><span data-stu-id="c0680-210">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0680-211">Связи</span><span class="sxs-lookup"><span data-stu-id="c0680-211">Relationships</span></span>
<span data-ttu-id="c0680-212">Нет</span><span class="sxs-lookup"><span data-stu-id="c0680-212">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0680-213">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0680-213">JSON Representation</span></span>
<span data-ttu-id="c0680-214">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0680-214">Here is a JSON representation of the resource.</span></span>
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



