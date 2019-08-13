---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 37d0f1d845891a397d5109a4d50d4de83b27f212
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332185"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="747de-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="747de-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="747de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="747de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="747de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="747de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="747de-106">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="747de-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="747de-107">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="747de-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="747de-108">Методы</span><span class="sxs-lookup"><span data-stu-id="747de-108">Methods</span></span>
|<span data-ttu-id="747de-109">Метод</span><span class="sxs-lookup"><span data-stu-id="747de-109">Method</span></span>|<span data-ttu-id="747de-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="747de-110">Return Type</span></span>|<span data-ttu-id="747de-111">Описание</span><span class="sxs-lookup"><span data-stu-id="747de-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="747de-112">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="747de-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="747de-113">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="747de-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="747de-114">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="747de-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="747de-115">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="747de-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="747de-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="747de-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="747de-117">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="747de-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="747de-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="747de-118">Properties</span></span>
|<span data-ttu-id="747de-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="747de-119">Property</span></span>|<span data-ttu-id="747de-120">Тип</span><span class="sxs-lookup"><span data-stu-id="747de-120">Type</span></span>|<span data-ttu-id="747de-121">Описание</span><span class="sxs-lookup"><span data-stu-id="747de-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="747de-122">displayName</span><span class="sxs-lookup"><span data-stu-id="747de-122">displayName</span></span>|<span data-ttu-id="747de-123">Строка</span><span class="sxs-lookup"><span data-stu-id="747de-123">String</span></span>|<span data-ttu-id="747de-124">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="747de-124">Policy display name.</span></span> <span data-ttu-id="747de-125">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="747de-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="747de-126">description</span><span class="sxs-lookup"><span data-stu-id="747de-126">description</span></span>|<span data-ttu-id="747de-127">String</span><span class="sxs-lookup"><span data-stu-id="747de-127">String</span></span>|<span data-ttu-id="747de-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="747de-128">The policy's description.</span></span> <span data-ttu-id="747de-129">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="747de-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="747de-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="747de-130">createdDateTime</span></span>|<span data-ttu-id="747de-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="747de-131">DateTimeOffset</span></span>|<span data-ttu-id="747de-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="747de-132">The date and time the policy was created.</span></span> <span data-ttu-id="747de-133">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="747de-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="747de-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="747de-134">lastModifiedDateTime</span></span>|<span data-ttu-id="747de-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="747de-135">DateTimeOffset</span></span>|<span data-ttu-id="747de-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="747de-136">Last time the policy was modified.</span></span> <span data-ttu-id="747de-137">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="747de-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="747de-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="747de-138">roleScopeTagIds</span></span>|<span data-ttu-id="747de-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="747de-139">String collection</span></span>|<span data-ttu-id="747de-140">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="747de-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="747de-141">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="747de-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="747de-142">id</span><span class="sxs-lookup"><span data-stu-id="747de-142">id</span></span>|<span data-ttu-id="747de-143">String</span><span class="sxs-lookup"><span data-stu-id="747de-143">String</span></span>|<span data-ttu-id="747de-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="747de-144">Key of the entity.</span></span> <span data-ttu-id="747de-145">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="747de-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="747de-146">version</span><span class="sxs-lookup"><span data-stu-id="747de-146">version</span></span>|<span data-ttu-id="747de-147">String</span><span class="sxs-lookup"><span data-stu-id="747de-147">String</span></span>|<span data-ttu-id="747de-148">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="747de-148">Version of the entity.</span></span> <span data-ttu-id="747de-149">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="747de-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="747de-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="747de-150">customSettings</span></span>|<span data-ttu-id="747de-151">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="747de-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="747de-152">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="747de-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="747de-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="747de-153">Relationships</span></span>
<span data-ttu-id="747de-154">Нет</span><span class="sxs-lookup"><span data-stu-id="747de-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="747de-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="747de-155">JSON Representation</span></span>
<span data-ttu-id="747de-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="747de-156">Here is a JSON representation of the resource.</span></span>
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



