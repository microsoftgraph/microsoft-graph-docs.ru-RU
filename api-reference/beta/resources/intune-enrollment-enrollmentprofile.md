---
title: Тип ресурса объекта enrollmentprofile
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b1b47d1479997f9f72bf7b7af4dca951b9e9d4bd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783496"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="c64c4-104">Тип ресурса объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="c64c4-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="c64c4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c64c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c64c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c64c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c64c4-107">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="c64c4-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="c64c4-108">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="c64c4-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="c64c4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c64c4-109">Methods</span></span>
|<span data-ttu-id="c64c4-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c64c4-110">Method</span></span>|<span data-ttu-id="c64c4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c64c4-111">Return Type</span></span>|<span data-ttu-id="c64c4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c64c4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c64c4-113">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="c64c4-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="c64c4-114">Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c64c4-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="c64c4-115">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c64c4-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="c64c4-116">Получение объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="c64c4-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|<span data-ttu-id="c64c4-117">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="c64c4-117">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="c64c4-118">Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c64c4-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c64c4-119">Создание объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="c64c4-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|<span data-ttu-id="c64c4-120">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="c64c4-120">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="c64c4-121">Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c64c4-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c64c4-122">Удаление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="c64c4-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="c64c4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c64c4-123">None</span></span>|<span data-ttu-id="c64c4-124">Удаляет объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c64c4-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="c64c4-125">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="c64c4-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|<span data-ttu-id="c64c4-126">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="c64c4-126">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="c64c4-127">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c64c4-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="c64c4-128">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="c64c4-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="c64c4-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c64c4-129">None</span></span>|<span data-ttu-id="c64c4-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c64c4-130">Not yet documented</span></span>|
|[<span data-ttu-id="c64c4-131">функция функция exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="c64c4-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="c64c4-132">String</span><span class="sxs-lookup"><span data-stu-id="c64c4-132">String</span></span>|<span data-ttu-id="c64c4-133">Экспорт конфигурации мобильного устройства</span><span class="sxs-lookup"><span data-stu-id="c64c4-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="c64c4-134">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="c64c4-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="c64c4-135">Нет</span><span class="sxs-lookup"><span data-stu-id="c64c4-135">None</span></span>|<span data-ttu-id="c64c4-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c64c4-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c64c4-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="c64c4-137">Properties</span></span>
|<span data-ttu-id="c64c4-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="c64c4-138">Property</span></span>|<span data-ttu-id="c64c4-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c64c4-139">Type</span></span>|<span data-ttu-id="c64c4-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c64c4-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c64c4-141">id</span><span class="sxs-lookup"><span data-stu-id="c64c4-141">id</span></span>|<span data-ttu-id="c64c4-142">Строка</span><span class="sxs-lookup"><span data-stu-id="c64c4-142">String</span></span>|<span data-ttu-id="c64c4-143">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="c64c4-143">The GUID for the object</span></span>|
|<span data-ttu-id="c64c4-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c64c4-144">displayName</span></span>|<span data-ttu-id="c64c4-145">Строка</span><span class="sxs-lookup"><span data-stu-id="c64c4-145">String</span></span>|<span data-ttu-id="c64c4-146">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="c64c4-146">Name of the profile</span></span>|
|<span data-ttu-id="c64c4-147">description</span><span class="sxs-lookup"><span data-stu-id="c64c4-147">description</span></span>|<span data-ttu-id="c64c4-148">String</span><span class="sxs-lookup"><span data-stu-id="c64c4-148">String</span></span>|<span data-ttu-id="c64c4-149">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="c64c4-149">Description of the profile</span></span>|
|<span data-ttu-id="c64c4-150">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="c64c4-150">requiresUserAuthentication</span></span>|<span data-ttu-id="c64c4-151">Логический</span><span class="sxs-lookup"><span data-stu-id="c64c4-151">Boolean</span></span>|<span data-ttu-id="c64c4-152">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="c64c4-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="c64c4-153">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="c64c4-153">configurationEndpointUrl</span></span>|<span data-ttu-id="c64c4-154">String</span><span class="sxs-lookup"><span data-stu-id="c64c4-154">String</span></span>|<span data-ttu-id="c64c4-155">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="c64c4-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="c64c4-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="c64c4-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="c64c4-157">Логический</span><span class="sxs-lookup"><span data-stu-id="c64c4-157">Boolean</span></span>|<span data-ttu-id="c64c4-158">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="c64c4-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="c64c4-159">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="c64c4-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="c64c4-160">Логический</span><span class="sxs-lookup"><span data-stu-id="c64c4-160">Boolean</span></span>|<span data-ttu-id="c64c4-161">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="c64c4-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c64c4-162">Связи</span><span class="sxs-lookup"><span data-stu-id="c64c4-162">Relationships</span></span>
<span data-ttu-id="c64c4-163">Нет</span><span class="sxs-lookup"><span data-stu-id="c64c4-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c64c4-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c64c4-164">JSON Representation</span></span>
<span data-ttu-id="c64c4-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c64c4-165">Here is a JSON representation of the resource.</span></span>
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



