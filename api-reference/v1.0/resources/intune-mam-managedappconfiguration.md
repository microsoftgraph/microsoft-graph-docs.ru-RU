---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86c6ecdcad64ae38887370101f96106a9b3aa816
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465512"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="0fe61-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fe61-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="0fe61-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fe61-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fe61-105">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="0fe61-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="0fe61-106">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0fe61-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0fe61-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0fe61-107">Methods</span></span>
|<span data-ttu-id="0fe61-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0fe61-108">Method</span></span>|<span data-ttu-id="0fe61-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0fe61-109">Return Type</span></span>|<span data-ttu-id="0fe61-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0fe61-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fe61-111">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="0fe61-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="0fe61-112">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fe61-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="0fe61-113">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0fe61-114">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fe61-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="0fe61-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fe61-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="0fe61-116">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fe61-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fe61-117">Properties</span></span>
|<span data-ttu-id="0fe61-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fe61-118">Property</span></span>|<span data-ttu-id="0fe61-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0fe61-119">Type</span></span>|<span data-ttu-id="0fe61-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0fe61-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fe61-121">displayName</span><span class="sxs-lookup"><span data-stu-id="0fe61-121">displayName</span></span>|<span data-ttu-id="0fe61-122">String</span><span class="sxs-lookup"><span data-stu-id="0fe61-122">String</span></span>|<span data-ttu-id="0fe61-123">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="0fe61-123">Policy display name.</span></span> <span data-ttu-id="0fe61-124">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0fe61-125">description</span><span class="sxs-lookup"><span data-stu-id="0fe61-125">description</span></span>|<span data-ttu-id="0fe61-126">String</span><span class="sxs-lookup"><span data-stu-id="0fe61-126">String</span></span>|<span data-ttu-id="0fe61-127">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="0fe61-127">The policy's description.</span></span> <span data-ttu-id="0fe61-128">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0fe61-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fe61-129">createdDateTime</span></span>|<span data-ttu-id="0fe61-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fe61-130">DateTimeOffset</span></span>|<span data-ttu-id="0fe61-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="0fe61-131">The date and time the policy was created.</span></span> <span data-ttu-id="0fe61-132">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0fe61-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fe61-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0fe61-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fe61-134">DateTimeOffset</span></span>|<span data-ttu-id="0fe61-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="0fe61-135">Last time the policy was modified.</span></span> <span data-ttu-id="0fe61-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0fe61-137">id</span><span class="sxs-lookup"><span data-stu-id="0fe61-137">id</span></span>|<span data-ttu-id="0fe61-138">Строка</span><span class="sxs-lookup"><span data-stu-id="0fe61-138">String</span></span>|<span data-ttu-id="0fe61-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0fe61-139">Key of the entity.</span></span> <span data-ttu-id="0fe61-140">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0fe61-141">version</span><span class="sxs-lookup"><span data-stu-id="0fe61-141">version</span></span>|<span data-ttu-id="0fe61-142">String</span><span class="sxs-lookup"><span data-stu-id="0fe61-142">String</span></span>|<span data-ttu-id="0fe61-143">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0fe61-143">Version of the entity.</span></span> <span data-ttu-id="0fe61-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0fe61-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0fe61-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="0fe61-145">customSettings</span></span>|<span data-ttu-id="0fe61-146">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0fe61-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0fe61-147">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="0fe61-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fe61-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="0fe61-148">Relationships</span></span>
<span data-ttu-id="0fe61-149">Нет</span><span class="sxs-lookup"><span data-stu-id="0fe61-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fe61-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0fe61-150">JSON Representation</span></span>
<span data-ttu-id="0fe61-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fe61-151">Here is a JSON representation of the resource.</span></span>
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



