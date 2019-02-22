---
title: Тип ресурса объекта enrollmentprofile
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d8947864611ac2c0d26256a5d739d41b86c383f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151179"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="7105c-104">Тип ресурса объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="7105c-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="7105c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7105c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7105c-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7105c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7105c-107">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="7105c-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="7105c-108">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="7105c-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="7105c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="7105c-109">Methods</span></span>
|<span data-ttu-id="7105c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="7105c-110">Method</span></span>|<span data-ttu-id="7105c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7105c-111">Return Type</span></span>|<span data-ttu-id="7105c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7105c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7105c-113">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="7105c-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="7105c-114">Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="7105c-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="7105c-115">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7105c-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="7105c-116">Получение объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="7105c-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|<span data-ttu-id="7105c-117">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="7105c-117">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="7105c-118">Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7105c-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="7105c-119">Создание объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="7105c-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|<span data-ttu-id="7105c-120">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="7105c-120">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="7105c-121">Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7105c-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="7105c-122">Удаление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="7105c-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="7105c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7105c-123">None</span></span>|<span data-ttu-id="7105c-124">Удаляет объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="7105c-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="7105c-125">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="7105c-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|<span data-ttu-id="7105c-126">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="7105c-126">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="7105c-127">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7105c-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="7105c-128">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="7105c-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="7105c-129">Нет</span><span class="sxs-lookup"><span data-stu-id="7105c-129">None</span></span>|<span data-ttu-id="7105c-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7105c-130">Not yet documented</span></span>|
|[<span data-ttu-id="7105c-131">функция функция exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="7105c-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="7105c-132">String</span><span class="sxs-lookup"><span data-stu-id="7105c-132">String</span></span>|<span data-ttu-id="7105c-133">Экспорт конфигурации мобильного устройства</span><span class="sxs-lookup"><span data-stu-id="7105c-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="7105c-134">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7105c-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="7105c-135">Нет</span><span class="sxs-lookup"><span data-stu-id="7105c-135">None</span></span>|<span data-ttu-id="7105c-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7105c-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7105c-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="7105c-137">Properties</span></span>
|<span data-ttu-id="7105c-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="7105c-138">Property</span></span>|<span data-ttu-id="7105c-139">Тип</span><span class="sxs-lookup"><span data-stu-id="7105c-139">Type</span></span>|<span data-ttu-id="7105c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="7105c-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7105c-141">id</span><span class="sxs-lookup"><span data-stu-id="7105c-141">id</span></span>|<span data-ttu-id="7105c-142">String</span><span class="sxs-lookup"><span data-stu-id="7105c-142">String</span></span>|<span data-ttu-id="7105c-143">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="7105c-143">The GUID for the object</span></span>|
|<span data-ttu-id="7105c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="7105c-144">displayName</span></span>|<span data-ttu-id="7105c-145">String</span><span class="sxs-lookup"><span data-stu-id="7105c-145">String</span></span>|<span data-ttu-id="7105c-146">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="7105c-146">Name of the profile</span></span>|
|<span data-ttu-id="7105c-147">description</span><span class="sxs-lookup"><span data-stu-id="7105c-147">description</span></span>|<span data-ttu-id="7105c-148">String</span><span class="sxs-lookup"><span data-stu-id="7105c-148">String</span></span>|<span data-ttu-id="7105c-149">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="7105c-149">Description of the profile</span></span>|
|<span data-ttu-id="7105c-150">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="7105c-150">requiresUserAuthentication</span></span>|<span data-ttu-id="7105c-151">Логический</span><span class="sxs-lookup"><span data-stu-id="7105c-151">Boolean</span></span>|<span data-ttu-id="7105c-152">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="7105c-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="7105c-153">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="7105c-153">configurationEndpointUrl</span></span>|<span data-ttu-id="7105c-154">String</span><span class="sxs-lookup"><span data-stu-id="7105c-154">String</span></span>|<span data-ttu-id="7105c-155">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="7105c-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="7105c-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="7105c-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="7105c-157">Логический</span><span class="sxs-lookup"><span data-stu-id="7105c-157">Boolean</span></span>|<span data-ttu-id="7105c-158">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="7105c-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="7105c-159">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="7105c-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="7105c-160">Логический</span><span class="sxs-lookup"><span data-stu-id="7105c-160">Boolean</span></span>|<span data-ttu-id="7105c-161">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="7105c-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="7105c-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="7105c-162">Relationships</span></span>
<span data-ttu-id="7105c-163">None</span><span class="sxs-lookup"><span data-stu-id="7105c-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7105c-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7105c-164">JSON Representation</span></span>
<span data-ttu-id="7105c-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7105c-165">Here is a JSON representation of the resource.</span></span>
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




