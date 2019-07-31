---
title: Тип ресурса объекта enrollmentprofile
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ccd3bfaea1d76c77bea62bfb3ebefaad827570e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999180"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="d0478-104">Тип ресурса объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="d0478-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="d0478-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0478-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0478-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0478-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0478-107">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="d0478-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="d0478-108">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="d0478-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="d0478-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d0478-109">Methods</span></span>
|<span data-ttu-id="d0478-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d0478-110">Method</span></span>|<span data-ttu-id="d0478-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d0478-111">Return Type</span></span>|<span data-ttu-id="d0478-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d0478-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0478-113">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="d0478-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="d0478-114">Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d0478-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="d0478-115">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d0478-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="d0478-116">Получение объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="d0478-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|<span data-ttu-id="d0478-117">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="d0478-117">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="d0478-118">Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d0478-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d0478-119">Создание объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="d0478-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|<span data-ttu-id="d0478-120">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="d0478-120">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="d0478-121">Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d0478-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d0478-122">Удаление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="d0478-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="d0478-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d0478-123">None</span></span>|<span data-ttu-id="d0478-124">Удаляет объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d0478-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="d0478-125">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="d0478-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|<span data-ttu-id="d0478-126">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="d0478-126">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="d0478-127">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d0478-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d0478-128">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="d0478-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="d0478-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d0478-129">None</span></span>|<span data-ttu-id="d0478-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d0478-130">Not yet documented</span></span>|
|[<span data-ttu-id="d0478-131">функция функция exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="d0478-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="d0478-132">String</span><span class="sxs-lookup"><span data-stu-id="d0478-132">String</span></span>|<span data-ttu-id="d0478-133">Экспорт конфигурации мобильного устройства</span><span class="sxs-lookup"><span data-stu-id="d0478-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="d0478-134">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="d0478-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="d0478-135">Нет</span><span class="sxs-lookup"><span data-stu-id="d0478-135">None</span></span>|<span data-ttu-id="d0478-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d0478-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d0478-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0478-137">Properties</span></span>
|<span data-ttu-id="d0478-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0478-138">Property</span></span>|<span data-ttu-id="d0478-139">Тип</span><span class="sxs-lookup"><span data-stu-id="d0478-139">Type</span></span>|<span data-ttu-id="d0478-140">Описание</span><span class="sxs-lookup"><span data-stu-id="d0478-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0478-141">id</span><span class="sxs-lookup"><span data-stu-id="d0478-141">id</span></span>|<span data-ttu-id="d0478-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d0478-142">String</span></span>|<span data-ttu-id="d0478-143">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="d0478-143">The GUID for the object</span></span>|
|<span data-ttu-id="d0478-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d0478-144">displayName</span></span>|<span data-ttu-id="d0478-145">Строка</span><span class="sxs-lookup"><span data-stu-id="d0478-145">String</span></span>|<span data-ttu-id="d0478-146">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="d0478-146">Name of the profile</span></span>|
|<span data-ttu-id="d0478-147">description</span><span class="sxs-lookup"><span data-stu-id="d0478-147">description</span></span>|<span data-ttu-id="d0478-148">String</span><span class="sxs-lookup"><span data-stu-id="d0478-148">String</span></span>|<span data-ttu-id="d0478-149">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="d0478-149">Description of the profile</span></span>|
|<span data-ttu-id="d0478-150">Рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="d0478-150">requiresUserAuthentication</span></span>|<span data-ttu-id="d0478-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0478-151">Boolean</span></span>|<span data-ttu-id="d0478-152">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="d0478-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="d0478-153">Конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="d0478-153">configurationEndpointUrl</span></span>|<span data-ttu-id="d0478-154">String</span><span class="sxs-lookup"><span data-stu-id="d0478-154">String</span></span>|<span data-ttu-id="d0478-155">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="d0478-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="d0478-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d0478-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d0478-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0478-157">Boolean</span></span>|<span data-ttu-id="d0478-158">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="d0478-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="d0478-159">Рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="d0478-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d0478-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0478-160">Boolean</span></span>|<span data-ttu-id="d0478-161">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="d0478-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0478-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="d0478-162">Relationships</span></span>
<span data-ttu-id="d0478-163">Нет</span><span class="sxs-lookup"><span data-stu-id="d0478-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0478-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0478-164">JSON Representation</span></span>
<span data-ttu-id="d0478-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0478-165">Here is a JSON representation of the resource.</span></span>
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





