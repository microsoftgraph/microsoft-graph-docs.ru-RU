---
title: Тип ресурса объекта enrollmentprofile
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 954f1d846b2af90598239d205970e3c2505f1fb1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460857"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="5a4f4-104">Тип ресурса объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="5a4f4-104">enrollmentProfile resource type</span></span>

<span data-ttu-id="5a4f4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a4f4-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a4f4-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a4f4-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a4f4-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a4f4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a4f4-108">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="5a4f4-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="5a4f4-109">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="5a4f4-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="5a4f4-110">Методы</span><span class="sxs-lookup"><span data-stu-id="5a4f4-110">Methods</span></span>
|<span data-ttu-id="5a4f4-111">Метод</span><span class="sxs-lookup"><span data-stu-id="5a4f4-111">Method</span></span>|<span data-ttu-id="5a4f4-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a4f4-112">Return Type</span></span>|<span data-ttu-id="5a4f4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5a4f4-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a4f4-114">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="5a4f4-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="5a4f4-115">Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5a4f4-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="5a4f4-116">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5a4f4-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="5a4f4-117">Получение объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="5a4f4-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|<span data-ttu-id="5a4f4-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="5a4f4-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="5a4f4-119">Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5a4f4-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5a4f4-120">Создание объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="5a4f4-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|<span data-ttu-id="5a4f4-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="5a4f4-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="5a4f4-122">Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5a4f4-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5a4f4-123">Удаление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="5a4f4-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="5a4f4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5a4f4-124">None</span></span>|<span data-ttu-id="5a4f4-125">Удаляет объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5a4f4-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="5a4f4-126">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="5a4f4-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|<span data-ttu-id="5a4f4-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="5a4f4-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="5a4f4-128">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5a4f4-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5a4f4-129">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="5a4f4-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="5a4f4-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5a4f4-130">None</span></span>|<span data-ttu-id="5a4f4-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5a4f4-131">Not yet documented</span></span>|
|[<span data-ttu-id="5a4f4-132">функция функция exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="5a4f4-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="5a4f4-133">String</span><span class="sxs-lookup"><span data-stu-id="5a4f4-133">String</span></span>|<span data-ttu-id="5a4f4-134">Экспорт конфигурации мобильного устройства</span><span class="sxs-lookup"><span data-stu-id="5a4f4-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="5a4f4-135">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5a4f4-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="5a4f4-136">Нет</span><span class="sxs-lookup"><span data-stu-id="5a4f4-136">None</span></span>|<span data-ttu-id="5a4f4-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5a4f4-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5a4f4-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a4f4-138">Properties</span></span>
|<span data-ttu-id="5a4f4-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a4f4-139">Property</span></span>|<span data-ttu-id="5a4f4-140">Тип</span><span class="sxs-lookup"><span data-stu-id="5a4f4-140">Type</span></span>|<span data-ttu-id="5a4f4-141">Описание</span><span class="sxs-lookup"><span data-stu-id="5a4f4-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a4f4-142">id</span><span class="sxs-lookup"><span data-stu-id="5a4f4-142">id</span></span>|<span data-ttu-id="5a4f4-143">Строка</span><span class="sxs-lookup"><span data-stu-id="5a4f4-143">String</span></span>|<span data-ttu-id="5a4f4-144">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="5a4f4-144">The GUID for the object</span></span>|
|<span data-ttu-id="5a4f4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5a4f4-145">displayName</span></span>|<span data-ttu-id="5a4f4-146">Строка</span><span class="sxs-lookup"><span data-stu-id="5a4f4-146">String</span></span>|<span data-ttu-id="5a4f4-147">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="5a4f4-147">Name of the profile</span></span>|
|<span data-ttu-id="5a4f4-148">description</span><span class="sxs-lookup"><span data-stu-id="5a4f4-148">description</span></span>|<span data-ttu-id="5a4f4-149">String</span><span class="sxs-lookup"><span data-stu-id="5a4f4-149">String</span></span>|<span data-ttu-id="5a4f4-150">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="5a4f4-150">Description of the profile</span></span>|
|<span data-ttu-id="5a4f4-151">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="5a4f4-151">requiresUserAuthentication</span></span>|<span data-ttu-id="5a4f4-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a4f4-152">Boolean</span></span>|<span data-ttu-id="5a4f4-153">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="5a4f4-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="5a4f4-154">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="5a4f4-154">configurationEndpointUrl</span></span>|<span data-ttu-id="5a4f4-155">String</span><span class="sxs-lookup"><span data-stu-id="5a4f4-155">String</span></span>|<span data-ttu-id="5a4f4-156">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="5a4f4-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="5a4f4-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="5a4f4-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="5a4f4-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a4f4-158">Boolean</span></span>|<span data-ttu-id="5a4f4-159">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="5a4f4-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="5a4f4-160">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="5a4f4-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="5a4f4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a4f4-161">Boolean</span></span>|<span data-ttu-id="5a4f4-162">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="5a4f4-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a4f4-163">Связи</span><span class="sxs-lookup"><span data-stu-id="5a4f4-163">Relationships</span></span>
<span data-ttu-id="5a4f4-164">Нет</span><span class="sxs-lookup"><span data-stu-id="5a4f4-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a4f4-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a4f4-165">JSON Representation</span></span>
<span data-ttu-id="5a4f4-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a4f4-166">Here is a JSON representation of the resource.</span></span>
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



