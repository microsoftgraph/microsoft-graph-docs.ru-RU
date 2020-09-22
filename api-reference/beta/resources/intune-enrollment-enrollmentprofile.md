---
title: Тип ресурса объекта enrollmentprofile
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8c8d132aca31abe7e90131509f73d9d7a15d0db7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080209"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="2dbf1-104">Тип ресурса объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="2dbf1-104">enrollmentProfile resource type</span></span>

<span data-ttu-id="2dbf1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dbf1-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2dbf1-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dbf1-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dbf1-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2dbf1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dbf1-108">Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены.</span><span class="sxs-lookup"><span data-stu-id="2dbf1-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="2dbf1-109">Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.</span><span class="sxs-lookup"><span data-stu-id="2dbf1-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="2dbf1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="2dbf1-110">Methods</span></span>
|<span data-ttu-id="2dbf1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="2dbf1-111">Method</span></span>|<span data-ttu-id="2dbf1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2dbf1-112">Return Type</span></span>|<span data-ttu-id="2dbf1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="2dbf1-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2dbf1-114">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="2dbf1-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="2dbf1-115">Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2dbf1-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="2dbf1-116">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2dbf1-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="2dbf1-117">Получение объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="2dbf1-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|<span data-ttu-id="2dbf1-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="2dbf1-118">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="2dbf1-119">Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2dbf1-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="2dbf1-120">Создание объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="2dbf1-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|<span data-ttu-id="2dbf1-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="2dbf1-121">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="2dbf1-122">Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2dbf1-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="2dbf1-123">Удаление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="2dbf1-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="2dbf1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="2dbf1-124">None</span></span>|<span data-ttu-id="2dbf1-125">Удаляет объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2dbf1-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="2dbf1-126">Обновление объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="2dbf1-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|<span data-ttu-id="2dbf1-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);</span><span class="sxs-lookup"><span data-stu-id="2dbf1-127">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|<span data-ttu-id="2dbf1-128">Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2dbf1-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="2dbf1-129">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="2dbf1-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="2dbf1-130">Нет</span><span class="sxs-lookup"><span data-stu-id="2dbf1-130">None</span></span>|<span data-ttu-id="2dbf1-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2dbf1-131">Not yet documented</span></span>|
|[<span data-ttu-id="2dbf1-132">функция функция exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="2dbf1-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="2dbf1-133">String</span><span class="sxs-lookup"><span data-stu-id="2dbf1-133">String</span></span>|<span data-ttu-id="2dbf1-134">Экспорт конфигурации мобильного устройства</span><span class="sxs-lookup"><span data-stu-id="2dbf1-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="2dbf1-135">Действие updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="2dbf1-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="2dbf1-136">Нет</span><span class="sxs-lookup"><span data-stu-id="2dbf1-136">None</span></span>|<span data-ttu-id="2dbf1-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2dbf1-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2dbf1-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dbf1-138">Properties</span></span>
|<span data-ttu-id="2dbf1-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dbf1-139">Property</span></span>|<span data-ttu-id="2dbf1-140">Тип</span><span class="sxs-lookup"><span data-stu-id="2dbf1-140">Type</span></span>|<span data-ttu-id="2dbf1-141">Описание</span><span class="sxs-lookup"><span data-stu-id="2dbf1-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dbf1-142">id</span><span class="sxs-lookup"><span data-stu-id="2dbf1-142">id</span></span>|<span data-ttu-id="2dbf1-143">String</span><span class="sxs-lookup"><span data-stu-id="2dbf1-143">String</span></span>|<span data-ttu-id="2dbf1-144">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="2dbf1-144">The GUID for the object</span></span>|
|<span data-ttu-id="2dbf1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2dbf1-145">displayName</span></span>|<span data-ttu-id="2dbf1-146">String</span><span class="sxs-lookup"><span data-stu-id="2dbf1-146">String</span></span>|<span data-ttu-id="2dbf1-147">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="2dbf1-147">Name of the profile</span></span>|
|<span data-ttu-id="2dbf1-148">description</span><span class="sxs-lookup"><span data-stu-id="2dbf1-148">description</span></span>|<span data-ttu-id="2dbf1-149">String</span><span class="sxs-lookup"><span data-stu-id="2dbf1-149">String</span></span>|<span data-ttu-id="2dbf1-150">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="2dbf1-150">Description of the profile</span></span>|
|<span data-ttu-id="2dbf1-151">рекуиресусераусентикатион</span><span class="sxs-lookup"><span data-stu-id="2dbf1-151">requiresUserAuthentication</span></span>|<span data-ttu-id="2dbf1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dbf1-152">Boolean</span></span>|<span data-ttu-id="2dbf1-153">Указывает, требуется ли для профиля проверка подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="2dbf1-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="2dbf1-154">конфигуратионендпоинтурл</span><span class="sxs-lookup"><span data-stu-id="2dbf1-154">configurationEndpointUrl</span></span>|<span data-ttu-id="2dbf1-155">String</span><span class="sxs-lookup"><span data-stu-id="2dbf1-155">String</span></span>|<span data-ttu-id="2dbf1-156">URL-адрес конечной точки конфигурации, используемый для регистрации</span><span class="sxs-lookup"><span data-stu-id="2dbf1-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="2dbf1-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2dbf1-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="2dbf1-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dbf1-158">Boolean</span></span>|<span data-ttu-id="2dbf1-159">Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.</span><span class="sxs-lookup"><span data-stu-id="2dbf1-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="2dbf1-160">рекуирекомпанипорталонсетупассистантенролледдевицес</span><span class="sxs-lookup"><span data-stu-id="2dbf1-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="2dbf1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dbf1-161">Boolean</span></span>|<span data-ttu-id="2dbf1-162">Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке</span><span class="sxs-lookup"><span data-stu-id="2dbf1-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dbf1-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="2dbf1-163">Relationships</span></span>
<span data-ttu-id="2dbf1-164">Нет</span><span class="sxs-lookup"><span data-stu-id="2dbf1-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dbf1-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2dbf1-165">JSON Representation</span></span>
<span data-ttu-id="2dbf1-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dbf1-166">Here is a JSON representation of the resource.</span></span>
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






