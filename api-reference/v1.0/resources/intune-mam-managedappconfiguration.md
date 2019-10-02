---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a133983c7bc58b4e0abacbfa336280a54c373df5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356396"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="8c135-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c135-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="8c135-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c135-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c135-105">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="8c135-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="8c135-106">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c135-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8c135-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8c135-107">Methods</span></span>
|<span data-ttu-id="8c135-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8c135-108">Method</span></span>|<span data-ttu-id="8c135-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c135-109">Return Type</span></span>|<span data-ttu-id="8c135-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c135-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c135-111">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8c135-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="8c135-112">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c135-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="8c135-113">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8c135-114">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c135-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="8c135-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c135-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="8c135-116">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c135-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c135-117">Properties</span></span>
|<span data-ttu-id="8c135-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c135-118">Property</span></span>|<span data-ttu-id="8c135-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8c135-119">Type</span></span>|<span data-ttu-id="8c135-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8c135-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c135-121">displayName</span><span class="sxs-lookup"><span data-stu-id="8c135-121">displayName</span></span>|<span data-ttu-id="8c135-122">Строка</span><span class="sxs-lookup"><span data-stu-id="8c135-122">String</span></span>|<span data-ttu-id="8c135-123">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="8c135-123">Policy display name.</span></span> <span data-ttu-id="8c135-124">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c135-125">description</span><span class="sxs-lookup"><span data-stu-id="8c135-125">description</span></span>|<span data-ttu-id="8c135-126">String</span><span class="sxs-lookup"><span data-stu-id="8c135-126">String</span></span>|<span data-ttu-id="8c135-127">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="8c135-127">The policy's description.</span></span> <span data-ttu-id="8c135-128">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c135-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c135-129">createdDateTime</span></span>|<span data-ttu-id="8c135-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c135-130">DateTimeOffset</span></span>|<span data-ttu-id="8c135-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="8c135-131">The date and time the policy was created.</span></span> <span data-ttu-id="8c135-132">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c135-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c135-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8c135-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c135-134">DateTimeOffset</span></span>|<span data-ttu-id="8c135-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="8c135-135">Last time the policy was modified.</span></span> <span data-ttu-id="8c135-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c135-137">id</span><span class="sxs-lookup"><span data-stu-id="8c135-137">id</span></span>|<span data-ttu-id="8c135-138">String</span><span class="sxs-lookup"><span data-stu-id="8c135-138">String</span></span>|<span data-ttu-id="8c135-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8c135-139">Key of the entity.</span></span> <span data-ttu-id="8c135-140">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c135-141">version</span><span class="sxs-lookup"><span data-stu-id="8c135-141">version</span></span>|<span data-ttu-id="8c135-142">String</span><span class="sxs-lookup"><span data-stu-id="8c135-142">String</span></span>|<span data-ttu-id="8c135-143">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8c135-143">Version of the entity.</span></span> <span data-ttu-id="8c135-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c135-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c135-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="8c135-145">customSettings</span></span>|<span data-ttu-id="8c135-146">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8c135-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8c135-147">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="8c135-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c135-148">Связи</span><span class="sxs-lookup"><span data-stu-id="8c135-148">Relationships</span></span>
<span data-ttu-id="8c135-149">Нет</span><span class="sxs-lookup"><span data-stu-id="8c135-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c135-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c135-150">JSON Representation</span></span>
<span data-ttu-id="8c135-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c135-151">Here is a JSON representation of the resource.</span></span>
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




