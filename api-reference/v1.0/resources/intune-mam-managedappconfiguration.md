---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffb8e5bbf86dceeedfe480676a18e70239a0d367
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754960"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="72b32-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="72b32-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="72b32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72b32-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72b32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72b32-106">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="72b32-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="72b32-107">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72b32-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="72b32-108">Методы</span><span class="sxs-lookup"><span data-stu-id="72b32-108">Methods</span></span>
|<span data-ttu-id="72b32-109">Метод</span><span class="sxs-lookup"><span data-stu-id="72b32-109">Method</span></span>|<span data-ttu-id="72b32-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72b32-110">Return Type</span></span>|<span data-ttu-id="72b32-111">Описание</span><span class="sxs-lookup"><span data-stu-id="72b32-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72b32-112">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="72b32-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="72b32-113">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72b32-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="72b32-114">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="72b32-115">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="72b32-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="72b32-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="72b32-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="72b32-117">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72b32-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="72b32-118">Properties</span></span>
|<span data-ttu-id="72b32-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="72b32-119">Property</span></span>|<span data-ttu-id="72b32-120">Тип</span><span class="sxs-lookup"><span data-stu-id="72b32-120">Type</span></span>|<span data-ttu-id="72b32-121">Описание</span><span class="sxs-lookup"><span data-stu-id="72b32-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72b32-122">displayName</span><span class="sxs-lookup"><span data-stu-id="72b32-122">displayName</span></span>|<span data-ttu-id="72b32-123">String</span><span class="sxs-lookup"><span data-stu-id="72b32-123">String</span></span>|<span data-ttu-id="72b32-124">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="72b32-124">Policy display name.</span></span> <span data-ttu-id="72b32-125">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="72b32-126">description</span><span class="sxs-lookup"><span data-stu-id="72b32-126">description</span></span>|<span data-ttu-id="72b32-127">String</span><span class="sxs-lookup"><span data-stu-id="72b32-127">String</span></span>|<span data-ttu-id="72b32-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="72b32-128">The policy's description.</span></span> <span data-ttu-id="72b32-129">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="72b32-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72b32-130">createdDateTime</span></span>|<span data-ttu-id="72b32-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b32-131">DateTimeOffset</span></span>|<span data-ttu-id="72b32-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="72b32-132">The date and time the policy was created.</span></span> <span data-ttu-id="72b32-133">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="72b32-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72b32-134">lastModifiedDateTime</span></span>|<span data-ttu-id="72b32-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b32-135">DateTimeOffset</span></span>|<span data-ttu-id="72b32-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="72b32-136">Last time the policy was modified.</span></span> <span data-ttu-id="72b32-137">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="72b32-138">id</span><span class="sxs-lookup"><span data-stu-id="72b32-138">id</span></span>|<span data-ttu-id="72b32-139">String</span><span class="sxs-lookup"><span data-stu-id="72b32-139">String</span></span>|<span data-ttu-id="72b32-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72b32-140">Key of the entity.</span></span> <span data-ttu-id="72b32-141">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="72b32-142">version</span><span class="sxs-lookup"><span data-stu-id="72b32-142">version</span></span>|<span data-ttu-id="72b32-143">String</span><span class="sxs-lookup"><span data-stu-id="72b32-143">String</span></span>|<span data-ttu-id="72b32-144">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="72b32-144">Version of the entity.</span></span> <span data-ttu-id="72b32-145">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="72b32-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="72b32-146">customSettings</span><span class="sxs-lookup"><span data-stu-id="72b32-146">customSettings</span></span>|<span data-ttu-id="72b32-147">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="72b32-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="72b32-148">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="72b32-148">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="72b32-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="72b32-149">Relationships</span></span>
<span data-ttu-id="72b32-150">Нет</span><span class="sxs-lookup"><span data-stu-id="72b32-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72b32-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72b32-151">JSON Representation</span></span>
<span data-ttu-id="72b32-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72b32-152">Here is a JSON representation of the resource.</span></span>
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




