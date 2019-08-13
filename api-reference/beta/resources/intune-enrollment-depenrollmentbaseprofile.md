---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 611df6a0aff2c2d3c0d6728aa9bbaa443d772a35
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328069"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="1fa96-104">Тип ресурса Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="1fa96-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="1fa96-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fa96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fa96-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fa96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fa96-107">Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="1fa96-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="1fa96-108">Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.</span><span class="sxs-lookup"><span data-stu-id="1fa96-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="1fa96-109">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1fa96-110">Методы</span><span class="sxs-lookup"><span data-stu-id="1fa96-110">Methods</span></span>
|<span data-ttu-id="1fa96-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1fa96-111">Method</span></span>|<span data-ttu-id="1fa96-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1fa96-112">Return Type</span></span>|<span data-ttu-id="1fa96-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa96-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1fa96-114">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="1fa96-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="1fa96-115">Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="1fa96-116">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1fa96-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="1fa96-117">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="1fa96-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="1fa96-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="1fa96-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="1fa96-119">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1fa96-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1fa96-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fa96-120">Properties</span></span>
|<span data-ttu-id="1fa96-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fa96-121">Property</span></span>|<span data-ttu-id="1fa96-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1fa96-122">Type</span></span>|<span data-ttu-id="1fa96-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa96-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fa96-124">id</span><span class="sxs-lookup"><span data-stu-id="1fa96-124">id</span></span>|<span data-ttu-id="1fa96-125">String</span><span class="sxs-lookup"><span data-stu-id="1fa96-125">String</span></span>|<span data-ttu-id="1fa96-126">GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fa96-127">displayName</span><span class="sxs-lookup"><span data-stu-id="1fa96-127">displayName</span></span>|<span data-ttu-id="1fa96-128">Строка</span><span class="sxs-lookup"><span data-stu-id="1fa96-128">String</span></span>|<span data-ttu-id="1fa96-129">Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fa96-130">description</span><span class="sxs-lookup"><span data-stu-id="1fa96-130">description</span></span>|<span data-ttu-id="1fa96-131">String</span><span class="sxs-lookup"><span data-stu-id="1fa96-131">String</span></span>|<span data-ttu-id="1fa96-132">Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fa96-133">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="1fa96-133">requiresUserAuthentication</span></span>|<span data-ttu-id="1fa96-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-134">Boolean</span></span>|<span data-ttu-id="1fa96-135">Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fa96-136">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="1fa96-136">configurationEndpointUrl</span></span>|<span data-ttu-id="1fa96-137">String</span><span class="sxs-lookup"><span data-stu-id="1fa96-137">String</span></span>|<span data-ttu-id="1fa96-138">URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fa96-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="1fa96-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="1fa96-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-140">Boolean</span></span>|<span data-ttu-id="1fa96-141">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="1fa96-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="1fa96-142">Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fa96-143">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="1fa96-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="1fa96-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-144">Boolean</span></span>|<span data-ttu-id="1fa96-145">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fa96-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fa96-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="1fa96-146">isDefault</span></span>|<span data-ttu-id="1fa96-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-147">Boolean</span></span>|<span data-ttu-id="1fa96-148">Указывает, является ли этот профиль профилем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="1fa96-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="1fa96-149">супервиседмодинаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-149">supervisedModeEnabled</span></span>|<span data-ttu-id="1fa96-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-150">Boolean</span></span>|<span data-ttu-id="1fa96-151">Защищенный режим, true для включения, false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="1fa96-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="1fa96-152">Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.</span><span class="sxs-lookup"><span data-stu-id="1fa96-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="1fa96-153">суппортдепартмент</span><span class="sxs-lookup"><span data-stu-id="1fa96-153">supportDepartment</span></span>|<span data-ttu-id="1fa96-154">String</span><span class="sxs-lookup"><span data-stu-id="1fa96-154">String</span></span>|<span data-ttu-id="1fa96-155">Сведения о отделе поддержки</span><span class="sxs-lookup"><span data-stu-id="1fa96-155">Support department information</span></span>|
|<span data-ttu-id="1fa96-156">пасскодедисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-156">passCodeDisabled</span></span>|<span data-ttu-id="1fa96-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-157">Boolean</span></span>|<span data-ttu-id="1fa96-158">Указывает, отключена ли область настройки секретного кода</span><span class="sxs-lookup"><span data-stu-id="1fa96-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-159">Обязательный</span><span class="sxs-lookup"><span data-stu-id="1fa96-159">isMandatory</span></span>|<span data-ttu-id="1fa96-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-160">Boolean</span></span>|<span data-ttu-id="1fa96-161">Указывает, является ли профиль обязательной</span><span class="sxs-lookup"><span data-stu-id="1fa96-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="1fa96-162">локатиондисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-162">locationDisabled</span></span>|<span data-ttu-id="1fa96-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-163">Boolean</span></span>|<span data-ttu-id="1fa96-164">Указывает, отключена ли область настройки службы расположения</span><span class="sxs-lookup"><span data-stu-id="1fa96-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-165">суппортфоненумбер</span><span class="sxs-lookup"><span data-stu-id="1fa96-165">supportPhoneNumber</span></span>|<span data-ttu-id="1fa96-166">String</span><span class="sxs-lookup"><span data-stu-id="1fa96-166">String</span></span>|<span data-ttu-id="1fa96-167">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="1fa96-167">Support phone number</span></span>|
|<span data-ttu-id="1fa96-168">профилеремовалдисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-168">profileRemovalDisabled</span></span>|<span data-ttu-id="1fa96-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-169">Boolean</span></span>|<span data-ttu-id="1fa96-170">Указывает, отключен ли параметр удаления профиля</span><span class="sxs-lookup"><span data-stu-id="1fa96-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="1fa96-171">рестореблоккед</span><span class="sxs-lookup"><span data-stu-id="1fa96-171">restoreBlocked</span></span>|<span data-ttu-id="1fa96-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-172">Boolean</span></span>|<span data-ttu-id="1fa96-173">Указывает, заблокирована ли область настроек восстановления</span><span class="sxs-lookup"><span data-stu-id="1fa96-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="1fa96-174">апплеиддисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-174">appleIdDisabled</span></span>|<span data-ttu-id="1fa96-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-175">Boolean</span></span>|<span data-ttu-id="1fa96-176">Указывает, отключена ли область настройки Apple ID</span><span class="sxs-lookup"><span data-stu-id="1fa96-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-177">термсандкондитионсдисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="1fa96-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-178">Boolean</span></span>|<span data-ttu-id="1fa96-179">Указывает, отключена ли область установки "условия и условия"</span><span class="sxs-lookup"><span data-stu-id="1fa96-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-180">таучиддисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-180">touchIdDisabled</span></span>|<span data-ttu-id="1fa96-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-181">Boolean</span></span>|<span data-ttu-id="1fa96-182">Указывает, отключена ли панель настройки сенсорного экрана</span><span class="sxs-lookup"><span data-stu-id="1fa96-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-183">апплепайдисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-183">applePayDisabled</span></span>|<span data-ttu-id="1fa96-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-184">Boolean</span></span>|<span data-ttu-id="1fa96-185">Указывает, отключена ли область настройки оплаты Apple</span><span class="sxs-lookup"><span data-stu-id="1fa96-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-186">зумдисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-186">zoomDisabled</span></span>|<span data-ttu-id="1fa96-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-187">Boolean</span></span>|<span data-ttu-id="1fa96-188">Указывает, отключена ли область настройки масштабирования</span><span class="sxs-lookup"><span data-stu-id="1fa96-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-189">сиридисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-189">siriDisabled</span></span>|<span data-ttu-id="1fa96-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-190">Boolean</span></span>|<span data-ttu-id="1fa96-191">Указывает, отключена ли область настройки Siri</span><span class="sxs-lookup"><span data-stu-id="1fa96-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-192">диагностиксдисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-192">diagnosticsDisabled</span></span>|<span data-ttu-id="1fa96-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-193">Boolean</span></span>|<span data-ttu-id="1fa96-194">Указывает, отключена ли область настройки диагностики</span><span class="sxs-lookup"><span data-stu-id="1fa96-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="1fa96-195">дисплайтонесетупдисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="1fa96-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-196">Boolean</span></span>|<span data-ttu-id="1fa96-197">Указывает, отключен ли экран установки дисплайтоне</span><span class="sxs-lookup"><span data-stu-id="1fa96-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="1fa96-198">приваципанедисаблед</span><span class="sxs-lookup"><span data-stu-id="1fa96-198">privacyPaneDisabled</span></span>|<span data-ttu-id="1fa96-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fa96-199">Boolean</span></span>|<span data-ttu-id="1fa96-200">Указывает, отключен ли экран конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="1fa96-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="1fa96-201">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="1fa96-201">deviceNameTemplate</span></span>|<span data-ttu-id="1fa96-202">String</span><span class="sxs-lookup"><span data-stu-id="1fa96-202">String</span></span>|<span data-ttu-id="1fa96-203">Задает шаблон литерала или имени.</span><span class="sxs-lookup"><span data-stu-id="1fa96-203">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fa96-204">Отношения</span><span class="sxs-lookup"><span data-stu-id="1fa96-204">Relationships</span></span>
<span data-ttu-id="1fa96-205">Нет</span><span class="sxs-lookup"><span data-stu-id="1fa96-205">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fa96-206">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fa96-206">JSON Representation</span></span>
<span data-ttu-id="1fa96-207">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fa96-207">Here is a JSON representation of the resource.</span></span>
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



