---
title: Тип ресурса enrollmentProfile
description: Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены. Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.
localization_priority: Normal
ms.openlocfilehash: 43aa6f5f3e8093da0c066012d763e5f0f6455da6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894308"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="53d7e-104">Тип ресурса enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="53d7e-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="53d7e-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53d7e-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53d7e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53d7e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53d7e-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="53d7e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53d7e-108">Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены.</span><span class="sxs-lookup"><span data-stu-id="53d7e-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="53d7e-109">Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="53d7e-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="53d7e-110">Методы</span><span class="sxs-lookup"><span data-stu-id="53d7e-110">Methods</span></span>
|<span data-ttu-id="53d7e-111">Метод</span><span class="sxs-lookup"><span data-stu-id="53d7e-111">Method</span></span>|<span data-ttu-id="53d7e-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53d7e-112">Return Type</span></span>|<span data-ttu-id="53d7e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="53d7e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53d7e-114">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="53d7e-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="53d7e-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="53d7e-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="53d7e-116">Свойства списка и связей объектов [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="53d7e-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="53d7e-117">Получение enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="53d7e-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|<span data-ttu-id="53d7e-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="53d7e-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="53d7e-119">Чтение свойства и связи объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="53d7e-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="53d7e-120">Создание enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="53d7e-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|<span data-ttu-id="53d7e-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="53d7e-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="53d7e-122">Создание нового объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="53d7e-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="53d7e-123">Удаление enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="53d7e-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="53d7e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="53d7e-124">None</span></span>|<span data-ttu-id="53d7e-125">Удаляет [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="53d7e-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="53d7e-126">Обновление enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="53d7e-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|<span data-ttu-id="53d7e-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="53d7e-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="53d7e-128">Обновление свойства объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="53d7e-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="53d7e-129">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="53d7e-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="53d7e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="53d7e-130">None</span></span>|<span data-ttu-id="53d7e-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="53d7e-131">Not yet documented</span></span>|
|[<span data-ttu-id="53d7e-132">функция exportMobileConfig</span><span class="sxs-lookup"><span data-stu-id="53d7e-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="53d7e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="53d7e-133">String</span></span>|<span data-ttu-id="53d7e-134">Экспорт конфигурации мобильных устройств</span><span class="sxs-lookup"><span data-stu-id="53d7e-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="53d7e-135">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="53d7e-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="53d7e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="53d7e-136">None</span></span>|<span data-ttu-id="53d7e-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="53d7e-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="53d7e-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="53d7e-138">Properties</span></span>
|<span data-ttu-id="53d7e-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="53d7e-139">Property</span></span>|<span data-ttu-id="53d7e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="53d7e-140">Type</span></span>|<span data-ttu-id="53d7e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="53d7e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53d7e-142">id</span><span class="sxs-lookup"><span data-stu-id="53d7e-142">id</span></span>|<span data-ttu-id="53d7e-143">Строка</span><span class="sxs-lookup"><span data-stu-id="53d7e-143">String</span></span>|<span data-ttu-id="53d7e-144">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="53d7e-144">The GUID for the object</span></span>|
|<span data-ttu-id="53d7e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="53d7e-145">displayName</span></span>|<span data-ttu-id="53d7e-146">Строка</span><span class="sxs-lookup"><span data-stu-id="53d7e-146">String</span></span>|<span data-ttu-id="53d7e-147">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="53d7e-147">Name of the profile</span></span>|
|<span data-ttu-id="53d7e-148">описание</span><span class="sxs-lookup"><span data-stu-id="53d7e-148">description</span></span>|<span data-ttu-id="53d7e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="53d7e-149">String</span></span>|<span data-ttu-id="53d7e-150">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="53d7e-150">Description of the profile</span></span>|
|<span data-ttu-id="53d7e-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="53d7e-151">requiresUserAuthentication</span></span>|<span data-ttu-id="53d7e-152">Логический</span><span class="sxs-lookup"><span data-stu-id="53d7e-152">Boolean</span></span>|<span data-ttu-id="53d7e-153">Указывает необходимость проверки подлинности пользователей в профиле</span><span class="sxs-lookup"><span data-stu-id="53d7e-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="53d7e-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="53d7e-154">configurationEndpointUrl</span></span>|<span data-ttu-id="53d7e-155">Строка</span><span class="sxs-lookup"><span data-stu-id="53d7e-155">String</span></span>|<span data-ttu-id="53d7e-156">URL-адрес конечной точки конфигурации для подачи заявок</span><span class="sxs-lookup"><span data-stu-id="53d7e-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="53d7e-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="53d7e-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="53d7e-158">Логический</span><span class="sxs-lookup"><span data-stu-id="53d7e-158">Boolean</span></span>|<span data-ttu-id="53d7e-159">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="53d7e-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53d7e-160">Связи</span><span class="sxs-lookup"><span data-stu-id="53d7e-160">Relationships</span></span>
<span data-ttu-id="53d7e-161">Нет</span><span class="sxs-lookup"><span data-stu-id="53d7e-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="53d7e-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53d7e-162">JSON Representation</span></span>
<span data-ttu-id="53d7e-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53d7e-163">Here is a JSON representation of the resource.</span></span>
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
  "enableAuthenticationViaCompanyPortal": true
}
```





