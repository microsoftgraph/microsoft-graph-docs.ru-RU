---
title: Тип ресурса объекта enrollmentprofile
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abc00f27ef65cdddfef30a06bef55a8fa44e488a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805525"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="4e7d2-104">Тип ресурса объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="4e7d2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e7d2-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e7d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e7d2-107">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="4e7d2-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="4e7d2-108">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="4e7d2-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="4e7d2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="4e7d2-109">Methods</span></span>
|<span data-ttu-id="4e7d2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4e7d2-110">Method</span></span>|<span data-ttu-id="4e7d2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e7d2-111">Return Type</span></span>|<span data-ttu-id="4e7d2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4e7d2-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4e7d2-113">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="4e7d2-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="4e7d2-114">Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="4e7d2-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="4e7d2-115">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4e7d2-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="4e7d2-116">Получение объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="4e7d2-117">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-117">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="4e7d2-118">Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4e7d2-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="4e7d2-119">Создание объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="4e7d2-120">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-120">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="4e7d2-121">Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4e7d2-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="4e7d2-122">Удаление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="4e7d2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4e7d2-123">None</span></span>|<span data-ttu-id="4e7d2-124">Удаляет объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="4e7d2-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="4e7d2-125">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="4e7d2-126">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-126">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="4e7d2-127">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4e7d2-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="4e7d2-128">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="4e7d2-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="4e7d2-129">Нет</span><span class="sxs-lookup"><span data-stu-id="4e7d2-129">None</span></span>|<span data-ttu-id="4e7d2-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4e7d2-130">Not yet documented</span></span>|
|[<span data-ttu-id="4e7d2-131">функция функция exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="4e7d2-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="4e7d2-132">String</span><span class="sxs-lookup"><span data-stu-id="4e7d2-132">String</span></span>|<span data-ttu-id="4e7d2-133">Экспорт конфигурации мобильного устройства</span><span class="sxs-lookup"><span data-stu-id="4e7d2-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="4e7d2-134">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="4e7d2-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="4e7d2-135">Нет</span><span class="sxs-lookup"><span data-stu-id="4e7d2-135">None</span></span>|<span data-ttu-id="4e7d2-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4e7d2-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4e7d2-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e7d2-137">Properties</span></span>
|<span data-ttu-id="4e7d2-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e7d2-138">Property</span></span>|<span data-ttu-id="4e7d2-139">Тип</span><span class="sxs-lookup"><span data-stu-id="4e7d2-139">Type</span></span>|<span data-ttu-id="4e7d2-140">Описание</span><span class="sxs-lookup"><span data-stu-id="4e7d2-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e7d2-141">id</span><span class="sxs-lookup"><span data-stu-id="4e7d2-141">id</span></span>|<span data-ttu-id="4e7d2-142">Строка</span><span class="sxs-lookup"><span data-stu-id="4e7d2-142">String</span></span>|<span data-ttu-id="4e7d2-143">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="4e7d2-143">The GUID for the object</span></span>|
|<span data-ttu-id="4e7d2-144">displayName</span><span class="sxs-lookup"><span data-stu-id="4e7d2-144">displayName</span></span>|<span data-ttu-id="4e7d2-145">String</span><span class="sxs-lookup"><span data-stu-id="4e7d2-145">String</span></span>|<span data-ttu-id="4e7d2-146">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="4e7d2-146">Name of the profile</span></span>|
|<span data-ttu-id="4e7d2-147">description</span><span class="sxs-lookup"><span data-stu-id="4e7d2-147">description</span></span>|<span data-ttu-id="4e7d2-148">String</span><span class="sxs-lookup"><span data-stu-id="4e7d2-148">String</span></span>|<span data-ttu-id="4e7d2-149">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="4e7d2-149">Description of the profile</span></span>|
|<span data-ttu-id="4e7d2-150">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="4e7d2-150">requiresUserAuthentication</span></span>|<span data-ttu-id="4e7d2-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e7d2-151">Boolean</span></span>|<span data-ttu-id="4e7d2-152">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="4e7d2-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="4e7d2-153">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="4e7d2-153">configurationEndpointUrl</span></span>|<span data-ttu-id="4e7d2-154">String</span><span class="sxs-lookup"><span data-stu-id="4e7d2-154">String</span></span>|<span data-ttu-id="4e7d2-155">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="4e7d2-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="4e7d2-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="4e7d2-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="4e7d2-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e7d2-157">Boolean</span></span>|<span data-ttu-id="4e7d2-158">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="4e7d2-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="4e7d2-159">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="4e7d2-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="4e7d2-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e7d2-160">Boolean</span></span>|<span data-ttu-id="4e7d2-161">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="4e7d2-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e7d2-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="4e7d2-162">Relationships</span></span>
<span data-ttu-id="4e7d2-163">Нет</span><span class="sxs-lookup"><span data-stu-id="4e7d2-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e7d2-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e7d2-164">JSON Representation</span></span>
<span data-ttu-id="4e7d2-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e7d2-165">Here is a JSON representation of the resource.</span></span>
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





