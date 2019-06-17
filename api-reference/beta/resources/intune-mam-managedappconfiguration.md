---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8d6fd389ef632aa1606fa8af070a0e83faf1d1b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991963"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="c80db-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c80db-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="c80db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c80db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c80db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c80db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c80db-106">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="c80db-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="c80db-107">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c80db-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c80db-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c80db-108">Methods</span></span>
|<span data-ttu-id="c80db-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c80db-109">Method</span></span>|<span data-ttu-id="c80db-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c80db-110">Return Type</span></span>|<span data-ttu-id="c80db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c80db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c80db-112">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="c80db-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="c80db-113">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c80db-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="c80db-114">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c80db-115">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c80db-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="c80db-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c80db-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="c80db-117">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c80db-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c80db-118">Properties</span></span>
|<span data-ttu-id="c80db-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c80db-119">Property</span></span>|<span data-ttu-id="c80db-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c80db-120">Type</span></span>|<span data-ttu-id="c80db-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c80db-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c80db-122">displayName</span><span class="sxs-lookup"><span data-stu-id="c80db-122">displayName</span></span>|<span data-ttu-id="c80db-123">Строка</span><span class="sxs-lookup"><span data-stu-id="c80db-123">String</span></span>|<span data-ttu-id="c80db-124">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="c80db-124">Policy display name.</span></span> <span data-ttu-id="c80db-125">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c80db-126">description</span><span class="sxs-lookup"><span data-stu-id="c80db-126">description</span></span>|<span data-ttu-id="c80db-127">String</span><span class="sxs-lookup"><span data-stu-id="c80db-127">String</span></span>|<span data-ttu-id="c80db-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="c80db-128">The policy's description.</span></span> <span data-ttu-id="c80db-129">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c80db-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c80db-130">createdDateTime</span></span>|<span data-ttu-id="c80db-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c80db-131">DateTimeOffset</span></span>|<span data-ttu-id="c80db-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="c80db-132">The date and time the policy was created.</span></span> <span data-ttu-id="c80db-133">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c80db-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c80db-134">lastModifiedDateTime</span></span>|<span data-ttu-id="c80db-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c80db-135">DateTimeOffset</span></span>|<span data-ttu-id="c80db-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="c80db-136">Last time the policy was modified.</span></span> <span data-ttu-id="c80db-137">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c80db-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c80db-138">roleScopeTagIds</span></span>|<span data-ttu-id="c80db-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c80db-139">String collection</span></span>|<span data-ttu-id="c80db-140">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c80db-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c80db-141">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c80db-142">id</span><span class="sxs-lookup"><span data-stu-id="c80db-142">id</span></span>|<span data-ttu-id="c80db-143">String</span><span class="sxs-lookup"><span data-stu-id="c80db-143">String</span></span>|<span data-ttu-id="c80db-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c80db-144">Key of the entity.</span></span> <span data-ttu-id="c80db-145">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c80db-146">version</span><span class="sxs-lookup"><span data-stu-id="c80db-146">version</span></span>|<span data-ttu-id="c80db-147">String</span><span class="sxs-lookup"><span data-stu-id="c80db-147">String</span></span>|<span data-ttu-id="c80db-148">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="c80db-148">Version of the entity.</span></span> <span data-ttu-id="c80db-149">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c80db-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c80db-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="c80db-150">customSettings</span></span>|<span data-ttu-id="c80db-151">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c80db-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c80db-152">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="c80db-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="c80db-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="c80db-153">Relationships</span></span>
<span data-ttu-id="c80db-154">Нет</span><span class="sxs-lookup"><span data-stu-id="c80db-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c80db-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c80db-155">JSON Representation</span></span>
<span data-ttu-id="c80db-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c80db-156">Here is a JSON representation of the resource.</span></span>
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





