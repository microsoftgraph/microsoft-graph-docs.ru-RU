---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48944007e33237e175822cfd2f5b076a5ddbe50e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524345"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="cd4c3-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4c3-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="cd4c3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cd4c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd4c3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd4c3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd4c3-107">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="cd4c3-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="cd4c3-108">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cd4c3-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cd4c3-109">Методы</span><span class="sxs-lookup"><span data-stu-id="cd4c3-109">Methods</span></span>
|<span data-ttu-id="cd4c3-110">Метод</span><span class="sxs-lookup"><span data-stu-id="cd4c3-110">Method</span></span>|<span data-ttu-id="cd4c3-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd4c3-111">Return Type</span></span>|<span data-ttu-id="cd4c3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cd4c3-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd4c3-113">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="cd4c3-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="cd4c3-114">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd4c3-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="cd4c3-115">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="cd4c3-116">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4c3-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="cd4c3-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4c3-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="cd4c3-118">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd4c3-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd4c3-119">Properties</span></span>
|<span data-ttu-id="cd4c3-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd4c3-120">Property</span></span>|<span data-ttu-id="cd4c3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cd4c3-121">Type</span></span>|<span data-ttu-id="cd4c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cd4c3-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd4c3-123">displayName</span><span class="sxs-lookup"><span data-stu-id="cd4c3-123">displayName</span></span>|<span data-ttu-id="cd4c3-124">Строка</span><span class="sxs-lookup"><span data-stu-id="cd4c3-124">String</span></span>|<span data-ttu-id="cd4c3-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-125">Policy display name.</span></span> <span data-ttu-id="cd4c3-126">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cd4c3-127">description</span><span class="sxs-lookup"><span data-stu-id="cd4c3-127">description</span></span>|<span data-ttu-id="cd4c3-128">String</span><span class="sxs-lookup"><span data-stu-id="cd4c3-128">String</span></span>|<span data-ttu-id="cd4c3-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-129">The policy's description.</span></span> <span data-ttu-id="cd4c3-130">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cd4c3-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd4c3-131">createdDateTime</span></span>|<span data-ttu-id="cd4c3-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd4c3-132">DateTimeOffset</span></span>|<span data-ttu-id="cd4c3-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-133">The date and time the policy was created.</span></span> <span data-ttu-id="cd4c3-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cd4c3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd4c3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cd4c3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd4c3-136">DateTimeOffset</span></span>|<span data-ttu-id="cd4c3-137">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-137">Last time the policy was modified.</span></span> <span data-ttu-id="cd4c3-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cd4c3-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cd4c3-139">roleScopeTagIds</span></span>|<span data-ttu-id="cd4c3-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cd4c3-140">String collection</span></span>|<span data-ttu-id="cd4c3-141">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cd4c3-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cd4c3-143">id</span><span class="sxs-lookup"><span data-stu-id="cd4c3-143">id</span></span>|<span data-ttu-id="cd4c3-144">String</span><span class="sxs-lookup"><span data-stu-id="cd4c3-144">String</span></span>|<span data-ttu-id="cd4c3-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-145">Key of the entity.</span></span> <span data-ttu-id="cd4c3-146">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cd4c3-147">version</span><span class="sxs-lookup"><span data-stu-id="cd4c3-147">version</span></span>|<span data-ttu-id="cd4c3-148">String</span><span class="sxs-lookup"><span data-stu-id="cd4c3-148">String</span></span>|<span data-ttu-id="cd4c3-149">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-149">Version of the entity.</span></span> <span data-ttu-id="cd4c3-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cd4c3-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="cd4c3-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="cd4c3-151">customSettings</span></span>|<span data-ttu-id="cd4c3-152">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="cd4c3-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="cd4c3-153">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="cd4c3-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd4c3-154">Связи</span><span class="sxs-lookup"><span data-stu-id="cd4c3-154">Relationships</span></span>
<span data-ttu-id="cd4c3-155">Нет</span><span class="sxs-lookup"><span data-stu-id="cd4c3-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd4c3-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd4c3-156">JSON Representation</span></span>
<span data-ttu-id="cd4c3-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd4c3-157">Here is a JSON representation of the resource.</span></span>
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



