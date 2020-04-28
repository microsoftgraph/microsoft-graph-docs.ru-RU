---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80484c3e5446cbb309ee3ae403475dedf075da56
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43373417"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="a0dd5-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0dd5-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="a0dd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0dd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0dd5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0dd5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0dd5-107">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="a0dd5-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="a0dd5-108">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a0dd5-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a0dd5-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a0dd5-109">Methods</span></span>
|<span data-ttu-id="a0dd5-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a0dd5-110">Method</span></span>|<span data-ttu-id="a0dd5-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0dd5-111">Return Type</span></span>|<span data-ttu-id="a0dd5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a0dd5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0dd5-113">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="a0dd5-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="a0dd5-114">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0dd5-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="a0dd5-115">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a0dd5-116">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0dd5-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="a0dd5-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0dd5-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="a0dd5-118">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0dd5-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0dd5-119">Properties</span></span>
|<span data-ttu-id="a0dd5-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0dd5-120">Property</span></span>|<span data-ttu-id="a0dd5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a0dd5-121">Type</span></span>|<span data-ttu-id="a0dd5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a0dd5-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0dd5-123">displayName</span><span class="sxs-lookup"><span data-stu-id="a0dd5-123">displayName</span></span>|<span data-ttu-id="a0dd5-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a0dd5-124">String</span></span>|<span data-ttu-id="a0dd5-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-125">Policy display name.</span></span> <span data-ttu-id="a0dd5-126">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0dd5-127">description</span><span class="sxs-lookup"><span data-stu-id="a0dd5-127">description</span></span>|<span data-ttu-id="a0dd5-128">String</span><span class="sxs-lookup"><span data-stu-id="a0dd5-128">String</span></span>|<span data-ttu-id="a0dd5-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-129">The policy's description.</span></span> <span data-ttu-id="a0dd5-130">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0dd5-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0dd5-131">createdDateTime</span></span>|<span data-ttu-id="a0dd5-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0dd5-132">DateTimeOffset</span></span>|<span data-ttu-id="a0dd5-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-133">The date and time the policy was created.</span></span> <span data-ttu-id="a0dd5-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0dd5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0dd5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a0dd5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0dd5-136">DateTimeOffset</span></span>|<span data-ttu-id="a0dd5-137">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-137">Last time the policy was modified.</span></span> <span data-ttu-id="a0dd5-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0dd5-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0dd5-139">roleScopeTagIds</span></span>|<span data-ttu-id="a0dd5-140">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a0dd5-140">String collection</span></span>|<span data-ttu-id="a0dd5-141">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0dd5-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0dd5-143">id</span><span class="sxs-lookup"><span data-stu-id="a0dd5-143">id</span></span>|<span data-ttu-id="a0dd5-144">String</span><span class="sxs-lookup"><span data-stu-id="a0dd5-144">String</span></span>|<span data-ttu-id="a0dd5-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-145">Key of the entity.</span></span> <span data-ttu-id="a0dd5-146">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0dd5-147">version</span><span class="sxs-lookup"><span data-stu-id="a0dd5-147">version</span></span>|<span data-ttu-id="a0dd5-148">String</span><span class="sxs-lookup"><span data-stu-id="a0dd5-148">String</span></span>|<span data-ttu-id="a0dd5-149">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-149">Version of the entity.</span></span> <span data-ttu-id="a0dd5-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0dd5-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0dd5-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="a0dd5-151">customSettings</span></span>|<span data-ttu-id="a0dd5-152">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a0dd5-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a0dd5-153">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="a0dd5-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0dd5-154">Связи</span><span class="sxs-lookup"><span data-stu-id="a0dd5-154">Relationships</span></span>
<span data-ttu-id="a0dd5-155">Нет</span><span class="sxs-lookup"><span data-stu-id="a0dd5-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0dd5-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0dd5-156">JSON Representation</span></span>
<span data-ttu-id="a0dd5-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0dd5-157">Here is a JSON representation of the resource.</span></span>
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



