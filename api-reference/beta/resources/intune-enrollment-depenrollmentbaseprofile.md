---
title: Тип ресурса depEnrollmentBaseProfile
description: Ресурс DepEnrollmentBaseProfile представляет профиля регистрации программы регистрации устройства Apple (DEP). Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423757"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="f1424-104">Тип ресурса depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f1424-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="f1424-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1424-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1424-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1424-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1424-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1424-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1424-108">Ресурс DepEnrollmentBaseProfile представляет профиля регистрации программы регистрации устройства Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="f1424-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="f1424-109">Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.</span><span class="sxs-lookup"><span data-stu-id="f1424-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="f1424-110">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f1424-111">Методы</span><span class="sxs-lookup"><span data-stu-id="f1424-111">Methods</span></span>
|<span data-ttu-id="f1424-112">Метод</span><span class="sxs-lookup"><span data-stu-id="f1424-112">Method</span></span>|<span data-ttu-id="f1424-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f1424-113">Return Type</span></span>|<span data-ttu-id="f1424-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f1424-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f1424-115">Список depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="f1424-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="f1424-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f1424-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="f1424-117">Свойства списка и связей объектов [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f1424-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="f1424-118">Получение depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f1424-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="f1424-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f1424-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="f1424-120">Чтение свойства и связи объекта [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f1424-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1424-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1424-121">Properties</span></span>
|<span data-ttu-id="f1424-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1424-122">Property</span></span>|<span data-ttu-id="f1424-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f1424-123">Type</span></span>|<span data-ttu-id="f1424-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f1424-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1424-125">id</span><span class="sxs-lookup"><span data-stu-id="f1424-125">id</span></span>|<span data-ttu-id="f1424-126">String</span><span class="sxs-lookup"><span data-stu-id="f1424-126">String</span></span>|<span data-ttu-id="f1424-127">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f1424-128">displayName</span><span class="sxs-lookup"><span data-stu-id="f1424-128">displayName</span></span>|<span data-ttu-id="f1424-129">String</span><span class="sxs-lookup"><span data-stu-id="f1424-129">String</span></span>|<span data-ttu-id="f1424-130">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f1424-131">description</span><span class="sxs-lookup"><span data-stu-id="f1424-131">description</span></span>|<span data-ttu-id="f1424-132">String</span><span class="sxs-lookup"><span data-stu-id="f1424-132">String</span></span>|<span data-ttu-id="f1424-133">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f1424-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f1424-134">requiresUserAuthentication</span></span>|<span data-ttu-id="f1424-135">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-135">Boolean</span></span>|<span data-ttu-id="f1424-136">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f1424-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f1424-137">configurationEndpointUrl</span></span>|<span data-ttu-id="f1424-138">String</span><span class="sxs-lookup"><span data-stu-id="f1424-138">String</span></span>|<span data-ttu-id="f1424-139">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f1424-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="f1424-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f1424-141">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-141">Boolean</span></span>|<span data-ttu-id="f1424-142">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="f1424-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f1424-143">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f1424-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="f1424-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f1424-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-145">Boolean</span></span>|<span data-ttu-id="f1424-146">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f1424-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f1424-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="f1424-147">isDefault</span></span>|<span data-ttu-id="f1424-148">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-148">Boolean</span></span>|<span data-ttu-id="f1424-149">Указывает, является ли профиля по умолчанию</span><span class="sxs-lookup"><span data-stu-id="f1424-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="f1424-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="f1424-150">supervisedModeEnabled</span></span>|<span data-ttu-id="f1424-151">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-151">Boolean</span></span>|<span data-ttu-id="f1424-152">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="f1424-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f1424-153">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="f1424-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="f1424-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="f1424-154">supportDepartment</span></span>|<span data-ttu-id="f1424-155">String</span><span class="sxs-lookup"><span data-stu-id="f1424-155">String</span></span>|<span data-ttu-id="f1424-156">Сведения о поддержке отдела</span><span class="sxs-lookup"><span data-stu-id="f1424-156">Support department information</span></span>|
|<span data-ttu-id="f1424-157">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-157">passCodeDisabled</span></span>|<span data-ttu-id="f1424-158">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-158">Boolean</span></span>|<span data-ttu-id="f1424-159">Указывает, если область настройки секретный код отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-160">isMandatory</span><span class="sxs-lookup"><span data-stu-id="f1424-160">isMandatory</span></span>|<span data-ttu-id="f1424-161">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-161">Boolean</span></span>|<span data-ttu-id="f1424-162">Указывает, является ли обязательных профилей</span><span class="sxs-lookup"><span data-stu-id="f1424-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="f1424-163">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-163">locationDisabled</span></span>|<span data-ttu-id="f1424-164">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-164">Boolean</span></span>|<span data-ttu-id="f1424-165">Указывает, если область настройки расположения службы отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-166">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f1424-166">supportPhoneNumber</span></span>|<span data-ttu-id="f1424-167">String</span><span class="sxs-lookup"><span data-stu-id="f1424-167">String</span></span>|<span data-ttu-id="f1424-168">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="f1424-168">Support phone number</span></span>|
|<span data-ttu-id="f1424-169">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-169">profileRemovalDisabled</span></span>|<span data-ttu-id="f1424-170">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-170">Boolean</span></span>|<span data-ttu-id="f1424-171">Указывает, если параметр удаления профиль отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="f1424-172">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f1424-172">restoreBlocked</span></span>|<span data-ttu-id="f1424-173">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-173">Boolean</span></span>|<span data-ttu-id="f1424-174">Указывает, если область настройки восстановления блокируется</span><span class="sxs-lookup"><span data-stu-id="f1424-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="f1424-175">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-175">appleIdDisabled</span></span>|<span data-ttu-id="f1424-176">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-176">Boolean</span></span>|<span data-ttu-id="f1424-177">Указывает, если область настройки идентификатор Apple отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-178">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f1424-179">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-179">Boolean</span></span>|<span data-ttu-id="f1424-180">Указывает, если отключено «Сроками и условиями» область настройки</span><span class="sxs-lookup"><span data-stu-id="f1424-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-181">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-181">touchIdDisabled</span></span>|<span data-ttu-id="f1424-182">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-182">Boolean</span></span>|<span data-ttu-id="f1424-183">Указывает, если область настройки идентификатор сенсорного ввода отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-184">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-184">applePayDisabled</span></span>|<span data-ttu-id="f1424-185">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-185">Boolean</span></span>|<span data-ttu-id="f1424-186">Указывает, если область настройки оплаты Apple отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-187">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-187">zoomDisabled</span></span>|<span data-ttu-id="f1424-188">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-188">Boolean</span></span>|<span data-ttu-id="f1424-189">Указывает, если область настройки масштаба отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-190">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-190">siriDisabled</span></span>|<span data-ttu-id="f1424-191">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-191">Boolean</span></span>|<span data-ttu-id="f1424-192">Указывает, если область настроек siri отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-193">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-193">diagnosticsDisabled</span></span>|<span data-ttu-id="f1424-194">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-194">Boolean</span></span>|<span data-ttu-id="f1424-195">Указывает, если область настройки диагностики отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="f1424-196">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="f1424-197">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-197">Boolean</span></span>|<span data-ttu-id="f1424-198">Указывает, если экран установки displaytone отключен</span><span class="sxs-lookup"><span data-stu-id="f1424-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="f1424-199">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="f1424-199">privacyPaneDisabled</span></span>|<span data-ttu-id="f1424-200">Логический</span><span class="sxs-lookup"><span data-stu-id="f1424-200">Boolean</span></span>|<span data-ttu-id="f1424-201">Указывает, если отключено экрана конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="f1424-201">Indicates if privacy screen is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1424-202">Отношения</span><span class="sxs-lookup"><span data-stu-id="f1424-202">Relationships</span></span>
<span data-ttu-id="f1424-203">Нет</span><span class="sxs-lookup"><span data-stu-id="f1424-203">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1424-204">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1424-204">JSON Representation</span></span>
<span data-ttu-id="f1424-205">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1424-205">Here is a JSON representation of the resource.</span></span>
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
  "privacyPaneDisabled": true
}
```




