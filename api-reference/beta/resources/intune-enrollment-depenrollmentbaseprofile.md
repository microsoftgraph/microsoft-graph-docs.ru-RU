---
title: Тип ресурса depEnrollmentBaseProfile
description: Ресурс DepEnrollmentBaseProfile представляет профиля регистрации программы регистрации устройства Apple (DEP). Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.
author: tfitzmac
ms.openlocfilehash: 26335fd3d35494b815dd43531ad54b4796dc861c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308374"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="c33be-104">Тип ресурса depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="c33be-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="c33be-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c33be-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c33be-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c33be-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c33be-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c33be-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c33be-108">Ресурс DepEnrollmentBaseProfile представляет профиля регистрации программы регистрации устройства Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="c33be-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="c33be-109">Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.</span><span class="sxs-lookup"><span data-stu-id="c33be-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="c33be-110">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c33be-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c33be-111">Методы</span><span class="sxs-lookup"><span data-stu-id="c33be-111">Methods</span></span>
|<span data-ttu-id="c33be-112">Метод</span><span class="sxs-lookup"><span data-stu-id="c33be-112">Method</span></span>|<span data-ttu-id="c33be-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c33be-113">Return Type</span></span>|<span data-ttu-id="c33be-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c33be-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c33be-115">Список depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="c33be-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="c33be-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c33be-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="c33be-117">Свойства списка и связей объектов [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c33be-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="c33be-118">Получение depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="c33be-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="c33be-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="c33be-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="c33be-120">Чтение свойства и связи объекта [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c33be-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c33be-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c33be-121">Properties</span></span>
|<span data-ttu-id="c33be-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c33be-122">Property</span></span>|<span data-ttu-id="c33be-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c33be-123">Type</span></span>|<span data-ttu-id="c33be-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c33be-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c33be-125">id</span><span class="sxs-lookup"><span data-stu-id="c33be-125">id</span></span>|<span data-ttu-id="c33be-126">Строка</span><span class="sxs-lookup"><span data-stu-id="c33be-126">String</span></span>|<span data-ttu-id="c33be-127">Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c33be-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c33be-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c33be-128">displayName</span></span>|<span data-ttu-id="c33be-129">Строка</span><span class="sxs-lookup"><span data-stu-id="c33be-129">String</span></span>|<span data-ttu-id="c33be-130">Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c33be-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c33be-131">описание</span><span class="sxs-lookup"><span data-stu-id="c33be-131">description</span></span>|<span data-ttu-id="c33be-132">Строка</span><span class="sxs-lookup"><span data-stu-id="c33be-132">String</span></span>|<span data-ttu-id="c33be-133">Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c33be-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c33be-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="c33be-134">requiresUserAuthentication</span></span>|<span data-ttu-id="c33be-135">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-135">Boolean</span></span>|<span data-ttu-id="c33be-136">Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c33be-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c33be-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="c33be-137">configurationEndpointUrl</span></span>|<span data-ttu-id="c33be-138">String.</span><span class="sxs-lookup"><span data-stu-id="c33be-138">String</span></span>|<span data-ttu-id="c33be-139">Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c33be-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c33be-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c33be-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c33be-141">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-141">Boolean</span></span>|<span data-ttu-id="c33be-142">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="c33be-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="c33be-143">Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c33be-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="c33be-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="c33be-144">isDefault</span></span>|<span data-ttu-id="c33be-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c33be-145">Boolean</span></span>|<span data-ttu-id="c33be-146">Указывает, является ли профиля по умолчанию</span><span class="sxs-lookup"><span data-stu-id="c33be-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="c33be-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="c33be-147">supervisedModeEnabled</span></span>|<span data-ttu-id="c33be-148">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-148">Boolean</span></span>|<span data-ttu-id="c33be-149">Режим контролируемом значение True для включения значение false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="c33be-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="c33be-150">Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="c33be-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="c33be-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="c33be-151">supportDepartment</span></span>|<span data-ttu-id="c33be-152">String.</span><span class="sxs-lookup"><span data-stu-id="c33be-152">String</span></span>|<span data-ttu-id="c33be-153">Сведения о поддержке отдела</span><span class="sxs-lookup"><span data-stu-id="c33be-153">Support department information</span></span>|
|<span data-ttu-id="c33be-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-154">passCodeDisabled</span></span>|<span data-ttu-id="c33be-155">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-155">Boolean</span></span>|<span data-ttu-id="c33be-156">Указывает, если область настройки секретный код отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="c33be-157">isMandatory</span></span>|<span data-ttu-id="c33be-158">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-158">Boolean</span></span>|<span data-ttu-id="c33be-159">Указывает, является ли обязательных профилей</span><span class="sxs-lookup"><span data-stu-id="c33be-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="c33be-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-160">locationDisabled</span></span>|<span data-ttu-id="c33be-161">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-161">Boolean</span></span>|<span data-ttu-id="c33be-162">Указывает, если область настройки расположения службы отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="c33be-163">supportPhoneNumber</span></span>|<span data-ttu-id="c33be-164">String.</span><span class="sxs-lookup"><span data-stu-id="c33be-164">String</span></span>|<span data-ttu-id="c33be-165">Номер телефона службы поддержки</span><span class="sxs-lookup"><span data-stu-id="c33be-165">Support phone number</span></span>|
|<span data-ttu-id="c33be-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-166">profileRemovalDisabled</span></span>|<span data-ttu-id="c33be-167">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-167">Boolean</span></span>|<span data-ttu-id="c33be-168">Указывает, если параметр удаления профиль отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="c33be-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="c33be-169">restoreBlocked</span></span>|<span data-ttu-id="c33be-170">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-170">Boolean</span></span>|<span data-ttu-id="c33be-171">Указывает, если область настройки восстановления блокируется</span><span class="sxs-lookup"><span data-stu-id="c33be-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="c33be-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-172">appleIdDisabled</span></span>|<span data-ttu-id="c33be-173">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-173">Boolean</span></span>|<span data-ttu-id="c33be-174">Указывает, если область настройки идентификатор Apple отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="c33be-176">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-176">Boolean</span></span>|<span data-ttu-id="c33be-177">Указывает, если отключено «Сроками и условиями» область настройки</span><span class="sxs-lookup"><span data-stu-id="c33be-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-178">touchIdDisabled</span></span>|<span data-ttu-id="c33be-179">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-179">Boolean</span></span>|<span data-ttu-id="c33be-180">Указывает, если область настройки идентификатор сенсорного ввода отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-181">applePayDisabled</span></span>|<span data-ttu-id="c33be-182">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-182">Boolean</span></span>|<span data-ttu-id="c33be-183">Указывает, если область настройки оплаты Apple отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-184">zoomDisabled</span></span>|<span data-ttu-id="c33be-185">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-185">Boolean</span></span>|<span data-ttu-id="c33be-186">Указывает, если область настройки масштаба отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-187">siriDisabled</span></span>|<span data-ttu-id="c33be-188">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-188">Boolean</span></span>|<span data-ttu-id="c33be-189">Указывает, если область настроек siri отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="c33be-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="c33be-190">diagnosticsDisabled</span></span>|<span data-ttu-id="c33be-191">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c33be-191">Boolean</span></span>|<span data-ttu-id="c33be-192">Указывает, если область настройки диагностики отключен</span><span class="sxs-lookup"><span data-stu-id="c33be-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="c33be-193">Связи</span><span class="sxs-lookup"><span data-stu-id="c33be-193">Relationships</span></span>
<span data-ttu-id="c33be-194">Нет</span><span class="sxs-lookup"><span data-stu-id="c33be-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c33be-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c33be-195">JSON Representation</span></span>
<span data-ttu-id="c33be-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c33be-196">Here is a JSON representation of the resource.</span></span>
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
  "diagnosticsDisabled": true
}
```





