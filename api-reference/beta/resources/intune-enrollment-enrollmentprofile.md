---
title: Тип ресурса enrollmentProfile
description: Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены. Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396842"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="45eb2-104">Тип ресурса enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="45eb2-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="45eb2-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45eb2-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45eb2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45eb2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45eb2-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45eb2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45eb2-108">Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены.</span><span class="sxs-lookup"><span data-stu-id="45eb2-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="45eb2-109">Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="45eb2-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="45eb2-110">Методы</span><span class="sxs-lookup"><span data-stu-id="45eb2-110">Methods</span></span>
|<span data-ttu-id="45eb2-111">Метод</span><span class="sxs-lookup"><span data-stu-id="45eb2-111">Method</span></span>|<span data-ttu-id="45eb2-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="45eb2-112">Return Type</span></span>|<span data-ttu-id="45eb2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="45eb2-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="45eb2-114">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="45eb2-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="45eb2-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="45eb2-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="45eb2-116">Свойства списка и связей объектов [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45eb2-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="45eb2-117">Получение enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="45eb2-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|<span data-ttu-id="45eb2-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="45eb2-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="45eb2-119">Чтение свойства и связи объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45eb2-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="45eb2-120">Создание enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="45eb2-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|<span data-ttu-id="45eb2-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="45eb2-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="45eb2-122">Создание нового объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45eb2-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="45eb2-123">Удаление enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="45eb2-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="45eb2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="45eb2-124">None</span></span>|<span data-ttu-id="45eb2-125">Удаляет [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="45eb2-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="45eb2-126">Обновление enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="45eb2-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|<span data-ttu-id="45eb2-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="45eb2-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="45eb2-128">Обновление свойства объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45eb2-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="45eb2-129">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="45eb2-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="45eb2-130">Нет</span><span class="sxs-lookup"><span data-stu-id="45eb2-130">None</span></span>|<span data-ttu-id="45eb2-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45eb2-131">Not yet documented</span></span>|
|[<span data-ttu-id="45eb2-132">функция exportMobileConfig</span><span class="sxs-lookup"><span data-stu-id="45eb2-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="45eb2-133">String</span><span class="sxs-lookup"><span data-stu-id="45eb2-133">String</span></span>|<span data-ttu-id="45eb2-134">Экспорт конфигурации мобильных устройств</span><span class="sxs-lookup"><span data-stu-id="45eb2-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="45eb2-135">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="45eb2-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="45eb2-136">Нет</span><span class="sxs-lookup"><span data-stu-id="45eb2-136">None</span></span>|<span data-ttu-id="45eb2-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45eb2-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="45eb2-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="45eb2-138">Properties</span></span>
|<span data-ttu-id="45eb2-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="45eb2-139">Property</span></span>|<span data-ttu-id="45eb2-140">Тип</span><span class="sxs-lookup"><span data-stu-id="45eb2-140">Type</span></span>|<span data-ttu-id="45eb2-141">Описание</span><span class="sxs-lookup"><span data-stu-id="45eb2-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45eb2-142">id</span><span class="sxs-lookup"><span data-stu-id="45eb2-142">id</span></span>|<span data-ttu-id="45eb2-143">Строка</span><span class="sxs-lookup"><span data-stu-id="45eb2-143">String</span></span>|<span data-ttu-id="45eb2-144">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="45eb2-144">The GUID for the object</span></span>|
|<span data-ttu-id="45eb2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="45eb2-145">displayName</span></span>|<span data-ttu-id="45eb2-146">String</span><span class="sxs-lookup"><span data-stu-id="45eb2-146">String</span></span>|<span data-ttu-id="45eb2-147">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="45eb2-147">Name of the profile</span></span>|
|<span data-ttu-id="45eb2-148">description</span><span class="sxs-lookup"><span data-stu-id="45eb2-148">description</span></span>|<span data-ttu-id="45eb2-149">String</span><span class="sxs-lookup"><span data-stu-id="45eb2-149">String</span></span>|<span data-ttu-id="45eb2-150">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="45eb2-150">Description of the profile</span></span>|
|<span data-ttu-id="45eb2-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="45eb2-151">requiresUserAuthentication</span></span>|<span data-ttu-id="45eb2-152">Логический</span><span class="sxs-lookup"><span data-stu-id="45eb2-152">Boolean</span></span>|<span data-ttu-id="45eb2-153">Указывает необходимость проверки подлинности пользователей в профиле</span><span class="sxs-lookup"><span data-stu-id="45eb2-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="45eb2-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="45eb2-154">configurationEndpointUrl</span></span>|<span data-ttu-id="45eb2-155">String</span><span class="sxs-lookup"><span data-stu-id="45eb2-155">String</span></span>|<span data-ttu-id="45eb2-156">URL-адрес конечной точки конфигурации для подачи заявок</span><span class="sxs-lookup"><span data-stu-id="45eb2-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="45eb2-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="45eb2-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="45eb2-158">Логический</span><span class="sxs-lookup"><span data-stu-id="45eb2-158">Boolean</span></span>|<span data-ttu-id="45eb2-159">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="45eb2-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="45eb2-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="45eb2-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="45eb2-161">Логический</span><span class="sxs-lookup"><span data-stu-id="45eb2-161">Boolean</span></span>|<span data-ttu-id="45eb2-162">Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки</span><span class="sxs-lookup"><span data-stu-id="45eb2-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="45eb2-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="45eb2-163">Relationships</span></span>
<span data-ttu-id="45eb2-164">Нет</span><span class="sxs-lookup"><span data-stu-id="45eb2-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45eb2-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45eb2-165">JSON Representation</span></span>
<span data-ttu-id="45eb2-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45eb2-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




