---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 557a314893faeb268ae21d13ec78a46bff9d6e0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809641"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="e2f0c-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2f0c-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="e2f0c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2f0c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2f0c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2f0c-107">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="e2f0c-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="e2f0c-108">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2f0c-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e2f0c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e2f0c-109">Methods</span></span>
|<span data-ttu-id="e2f0c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e2f0c-110">Method</span></span>|<span data-ttu-id="e2f0c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e2f0c-111">Return Type</span></span>|<span data-ttu-id="e2f0c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e2f0c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2f0c-113">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="e2f0c-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="e2f0c-114">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2f0c-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="e2f0c-115">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e2f0c-116">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2f0c-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="e2f0c-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2f0c-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="e2f0c-118">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2f0c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2f0c-119">Properties</span></span>
|<span data-ttu-id="e2f0c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2f0c-120">Property</span></span>|<span data-ttu-id="e2f0c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e2f0c-121">Type</span></span>|<span data-ttu-id="e2f0c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e2f0c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2f0c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="e2f0c-123">displayName</span></span>|<span data-ttu-id="e2f0c-124">Строка</span><span class="sxs-lookup"><span data-stu-id="e2f0c-124">String</span></span>|<span data-ttu-id="e2f0c-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-125">Policy display name.</span></span> <span data-ttu-id="e2f0c-126">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e2f0c-127">описание</span><span class="sxs-lookup"><span data-stu-id="e2f0c-127">description</span></span>|<span data-ttu-id="e2f0c-128">Строка</span><span class="sxs-lookup"><span data-stu-id="e2f0c-128">String</span></span>|<span data-ttu-id="e2f0c-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-129">The policy's description.</span></span> <span data-ttu-id="e2f0c-130">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e2f0c-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f0c-131">createdDateTime</span></span>|<span data-ttu-id="e2f0c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f0c-132">DateTimeOffset</span></span>|<span data-ttu-id="e2f0c-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-133">The date and time the policy was created.</span></span> <span data-ttu-id="e2f0c-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e2f0c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f0c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e2f0c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f0c-136">DateTimeOffset</span></span>|<span data-ttu-id="e2f0c-137">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-137">Last time the policy was modified.</span></span> <span data-ttu-id="e2f0c-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e2f0c-139">id</span><span class="sxs-lookup"><span data-stu-id="e2f0c-139">id</span></span>|<span data-ttu-id="e2f0c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e2f0c-140">String</span></span>|<span data-ttu-id="e2f0c-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-141">Key of the entity.</span></span> <span data-ttu-id="e2f0c-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e2f0c-143">version</span><span class="sxs-lookup"><span data-stu-id="e2f0c-143">version</span></span>|<span data-ttu-id="e2f0c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="e2f0c-144">String</span></span>|<span data-ttu-id="e2f0c-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-145">Version of the entity.</span></span> <span data-ttu-id="e2f0c-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e2f0c-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e2f0c-147">customSettings</span><span class="sxs-lookup"><span data-stu-id="e2f0c-147">customSettings</span></span>|<span data-ttu-id="e2f0c-148">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e2f0c-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e2f0c-149">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="e2f0c-149">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2f0c-150">Связи</span><span class="sxs-lookup"><span data-stu-id="e2f0c-150">Relationships</span></span>
<span data-ttu-id="e2f0c-151">Нет</span><span class="sxs-lookup"><span data-stu-id="e2f0c-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2f0c-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2f0c-152">JSON Representation</span></span>
<span data-ttu-id="e2f0c-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2f0c-153">Here is a JSON representation of the resource.</span></span>
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





