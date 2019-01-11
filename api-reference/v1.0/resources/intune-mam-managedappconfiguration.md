---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b3acf921f76e34e21427364ef84d1647cc7d0f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861322"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="81e0a-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81e0a-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="81e0a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81e0a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81e0a-105">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="81e0a-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="81e0a-106">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="81e0a-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="81e0a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="81e0a-107">Methods</span></span>
|<span data-ttu-id="81e0a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="81e0a-108">Method</span></span>|<span data-ttu-id="81e0a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81e0a-109">Return Type</span></span>|<span data-ttu-id="81e0a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="81e0a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81e0a-111">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="81e0a-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="81e0a-112">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81e0a-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="81e0a-113">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="81e0a-114">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81e0a-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="81e0a-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="81e0a-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="81e0a-116">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81e0a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="81e0a-117">Properties</span></span>
|<span data-ttu-id="81e0a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="81e0a-118">Property</span></span>|<span data-ttu-id="81e0a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="81e0a-119">Type</span></span>|<span data-ttu-id="81e0a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="81e0a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e0a-121">displayName</span><span class="sxs-lookup"><span data-stu-id="81e0a-121">displayName</span></span>|<span data-ttu-id="81e0a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="81e0a-122">String</span></span>|<span data-ttu-id="81e0a-123">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="81e0a-123">Policy display name.</span></span> <span data-ttu-id="81e0a-124">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e0a-125">описание</span><span class="sxs-lookup"><span data-stu-id="81e0a-125">description</span></span>|<span data-ttu-id="81e0a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="81e0a-126">String</span></span>|<span data-ttu-id="81e0a-127">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="81e0a-127">The policy's description.</span></span> <span data-ttu-id="81e0a-128">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e0a-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81e0a-129">createdDateTime</span></span>|<span data-ttu-id="81e0a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81e0a-130">DateTimeOffset</span></span>|<span data-ttu-id="81e0a-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="81e0a-131">The date and time the policy was created.</span></span> <span data-ttu-id="81e0a-132">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e0a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81e0a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="81e0a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81e0a-134">DateTimeOffset</span></span>|<span data-ttu-id="81e0a-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="81e0a-135">Last time the policy was modified.</span></span> <span data-ttu-id="81e0a-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e0a-137">id</span><span class="sxs-lookup"><span data-stu-id="81e0a-137">id</span></span>|<span data-ttu-id="81e0a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="81e0a-138">String</span></span>|<span data-ttu-id="81e0a-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="81e0a-139">Key of the entity.</span></span> <span data-ttu-id="81e0a-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e0a-141">version</span><span class="sxs-lookup"><span data-stu-id="81e0a-141">version</span></span>|<span data-ttu-id="81e0a-142">Строка</span><span class="sxs-lookup"><span data-stu-id="81e0a-142">String</span></span>|<span data-ttu-id="81e0a-143">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="81e0a-143">Version of the entity.</span></span> <span data-ttu-id="81e0a-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="81e0a-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="81e0a-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="81e0a-145">customSettings</span></span>|<span data-ttu-id="81e0a-146">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="81e0a-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="81e0a-147">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="81e0a-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="81e0a-148">Связи</span><span class="sxs-lookup"><span data-stu-id="81e0a-148">Relationships</span></span>
<span data-ttu-id="81e0a-149">Нет</span><span class="sxs-lookup"><span data-stu-id="81e0a-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81e0a-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81e0a-150">JSON Representation</span></span>
<span data-ttu-id="81e0a-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81e0a-151">Here is a JSON representation of the resource.</span></span>
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



