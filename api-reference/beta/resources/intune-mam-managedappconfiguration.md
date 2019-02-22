---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c8db1f356890dc478833e7b77267a218f08bbc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148086"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="f052e-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f052e-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="f052e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f052e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f052e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f052e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f052e-106">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="f052e-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="f052e-107">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f052e-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f052e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f052e-108">Methods</span></span>
|<span data-ttu-id="f052e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f052e-109">Method</span></span>|<span data-ttu-id="f052e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f052e-110">Return Type</span></span>|<span data-ttu-id="f052e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f052e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f052e-112">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="f052e-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="f052e-113">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f052e-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="f052e-114">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f052e-115">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f052e-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="f052e-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f052e-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="f052e-117">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f052e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f052e-118">Properties</span></span>
|<span data-ttu-id="f052e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f052e-119">Property</span></span>|<span data-ttu-id="f052e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f052e-120">Type</span></span>|<span data-ttu-id="f052e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f052e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f052e-122">displayName</span><span class="sxs-lookup"><span data-stu-id="f052e-122">displayName</span></span>|<span data-ttu-id="f052e-123">String</span><span class="sxs-lookup"><span data-stu-id="f052e-123">String</span></span>|<span data-ttu-id="f052e-124">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="f052e-124">Policy display name.</span></span> <span data-ttu-id="f052e-125">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f052e-126">description</span><span class="sxs-lookup"><span data-stu-id="f052e-126">description</span></span>|<span data-ttu-id="f052e-127">String</span><span class="sxs-lookup"><span data-stu-id="f052e-127">String</span></span>|<span data-ttu-id="f052e-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="f052e-128">The policy's description.</span></span> <span data-ttu-id="f052e-129">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f052e-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f052e-130">createdDateTime</span></span>|<span data-ttu-id="f052e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f052e-131">DateTimeOffset</span></span>|<span data-ttu-id="f052e-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="f052e-132">The date and time the policy was created.</span></span> <span data-ttu-id="f052e-133">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f052e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f052e-134">lastModifiedDateTime</span></span>|<span data-ttu-id="f052e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f052e-135">DateTimeOffset</span></span>|<span data-ttu-id="f052e-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="f052e-136">Last time the policy was modified.</span></span> <span data-ttu-id="f052e-137">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f052e-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f052e-138">roleScopeTagIds</span></span>|<span data-ttu-id="f052e-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f052e-139">String collection</span></span>|<span data-ttu-id="f052e-140">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f052e-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f052e-141">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f052e-142">id</span><span class="sxs-lookup"><span data-stu-id="f052e-142">id</span></span>|<span data-ttu-id="f052e-143">String</span><span class="sxs-lookup"><span data-stu-id="f052e-143">String</span></span>|<span data-ttu-id="f052e-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f052e-144">Key of the entity.</span></span> <span data-ttu-id="f052e-145">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f052e-146">version</span><span class="sxs-lookup"><span data-stu-id="f052e-146">version</span></span>|<span data-ttu-id="f052e-147">Строка</span><span class="sxs-lookup"><span data-stu-id="f052e-147">String</span></span>|<span data-ttu-id="f052e-148">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="f052e-148">Version of the entity.</span></span> <span data-ttu-id="f052e-149">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f052e-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="f052e-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="f052e-150">customSettings</span></span>|<span data-ttu-id="f052e-151">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f052e-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f052e-152">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="f052e-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="f052e-153">Связи</span><span class="sxs-lookup"><span data-stu-id="f052e-153">Relationships</span></span>
<span data-ttu-id="f052e-154">Нет</span><span class="sxs-lookup"><span data-stu-id="f052e-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f052e-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f052e-155">JSON Representation</span></span>
<span data-ttu-id="f052e-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f052e-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




