---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc34ab5464b1da8140d9d93f95ce1b34ab9ec9b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030439"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="70d4c-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="70d4c-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="70d4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70d4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70d4c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70d4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70d4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70d4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70d4c-107">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="70d4c-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="70d4c-108">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="70d4c-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="70d4c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="70d4c-109">Methods</span></span>
|<span data-ttu-id="70d4c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="70d4c-110">Method</span></span>|<span data-ttu-id="70d4c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70d4c-111">Return Type</span></span>|<span data-ttu-id="70d4c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="70d4c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70d4c-113">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="70d4c-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="70d4c-114">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="70d4c-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="70d4c-115">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="70d4c-116">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="70d4c-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="70d4c-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="70d4c-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="70d4c-118">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70d4c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="70d4c-119">Properties</span></span>
|<span data-ttu-id="70d4c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="70d4c-120">Property</span></span>|<span data-ttu-id="70d4c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="70d4c-121">Type</span></span>|<span data-ttu-id="70d4c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="70d4c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70d4c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="70d4c-123">displayName</span></span>|<span data-ttu-id="70d4c-124">String</span><span class="sxs-lookup"><span data-stu-id="70d4c-124">String</span></span>|<span data-ttu-id="70d4c-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="70d4c-125">Policy display name.</span></span> <span data-ttu-id="70d4c-126">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="70d4c-127">description</span><span class="sxs-lookup"><span data-stu-id="70d4c-127">description</span></span>|<span data-ttu-id="70d4c-128">String</span><span class="sxs-lookup"><span data-stu-id="70d4c-128">String</span></span>|<span data-ttu-id="70d4c-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="70d4c-129">The policy's description.</span></span> <span data-ttu-id="70d4c-130">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="70d4c-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70d4c-131">createdDateTime</span></span>|<span data-ttu-id="70d4c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70d4c-132">DateTimeOffset</span></span>|<span data-ttu-id="70d4c-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="70d4c-133">The date and time the policy was created.</span></span> <span data-ttu-id="70d4c-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="70d4c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70d4c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="70d4c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70d4c-136">DateTimeOffset</span></span>|<span data-ttu-id="70d4c-137">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="70d4c-137">Last time the policy was modified.</span></span> <span data-ttu-id="70d4c-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="70d4c-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70d4c-139">roleScopeTagIds</span></span>|<span data-ttu-id="70d4c-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="70d4c-140">String collection</span></span>|<span data-ttu-id="70d4c-141">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="70d4c-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="70d4c-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="70d4c-143">id</span><span class="sxs-lookup"><span data-stu-id="70d4c-143">id</span></span>|<span data-ttu-id="70d4c-144">String</span><span class="sxs-lookup"><span data-stu-id="70d4c-144">String</span></span>|<span data-ttu-id="70d4c-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="70d4c-145">Key of the entity.</span></span> <span data-ttu-id="70d4c-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="70d4c-147">version</span><span class="sxs-lookup"><span data-stu-id="70d4c-147">version</span></span>|<span data-ttu-id="70d4c-148">String</span><span class="sxs-lookup"><span data-stu-id="70d4c-148">String</span></span>|<span data-ttu-id="70d4c-149">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="70d4c-149">Version of the entity.</span></span> <span data-ttu-id="70d4c-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70d4c-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="70d4c-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="70d4c-151">customSettings</span></span>|<span data-ttu-id="70d4c-152">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="70d4c-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="70d4c-153">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="70d4c-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="70d4c-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="70d4c-154">Relationships</span></span>
<span data-ttu-id="70d4c-155">Нет</span><span class="sxs-lookup"><span data-stu-id="70d4c-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70d4c-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70d4c-156">JSON Representation</span></span>
<span data-ttu-id="70d4c-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70d4c-157">Here is a JSON representation of the resource.</span></span>
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






