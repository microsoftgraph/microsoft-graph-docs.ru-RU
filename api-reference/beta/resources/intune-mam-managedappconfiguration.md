---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67b445c5f7882bb4befc3e2c5cc46e26c5cf50fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405676"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="a0a14-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0a14-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="a0a14-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a0a14-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0a14-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0a14-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0a14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0a14-107">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="a0a14-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="a0a14-108">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a0a14-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a0a14-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a0a14-109">Methods</span></span>
|<span data-ttu-id="a0a14-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a0a14-110">Method</span></span>|<span data-ttu-id="a0a14-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0a14-111">Return Type</span></span>|<span data-ttu-id="a0a14-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a14-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0a14-113">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="a0a14-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="a0a14-114">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0a14-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="a0a14-115">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a0a14-116">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0a14-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="a0a14-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0a14-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="a0a14-118">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0a14-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0a14-119">Properties</span></span>
|<span data-ttu-id="a0a14-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0a14-120">Property</span></span>|<span data-ttu-id="a0a14-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a0a14-121">Type</span></span>|<span data-ttu-id="a0a14-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a0a14-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0a14-123">displayName</span><span class="sxs-lookup"><span data-stu-id="a0a14-123">displayName</span></span>|<span data-ttu-id="a0a14-124">String</span><span class="sxs-lookup"><span data-stu-id="a0a14-124">String</span></span>|<span data-ttu-id="a0a14-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="a0a14-125">Policy display name.</span></span> <span data-ttu-id="a0a14-126">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0a14-127">description</span><span class="sxs-lookup"><span data-stu-id="a0a14-127">description</span></span>|<span data-ttu-id="a0a14-128">String</span><span class="sxs-lookup"><span data-stu-id="a0a14-128">String</span></span>|<span data-ttu-id="a0a14-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="a0a14-129">The policy's description.</span></span> <span data-ttu-id="a0a14-130">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0a14-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0a14-131">createdDateTime</span></span>|<span data-ttu-id="a0a14-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0a14-132">DateTimeOffset</span></span>|<span data-ttu-id="a0a14-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="a0a14-133">The date and time the policy was created.</span></span> <span data-ttu-id="a0a14-134">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0a14-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0a14-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a0a14-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0a14-136">DateTimeOffset</span></span>|<span data-ttu-id="a0a14-137">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="a0a14-137">Last time the policy was modified.</span></span> <span data-ttu-id="a0a14-138">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0a14-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0a14-139">roleScopeTagIds</span></span>|<span data-ttu-id="a0a14-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a0a14-140">String collection</span></span>|<span data-ttu-id="a0a14-141">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a0a14-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0a14-142">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0a14-143">id</span><span class="sxs-lookup"><span data-stu-id="a0a14-143">id</span></span>|<span data-ttu-id="a0a14-144">String</span><span class="sxs-lookup"><span data-stu-id="a0a14-144">String</span></span>|<span data-ttu-id="a0a14-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a0a14-145">Key of the entity.</span></span> <span data-ttu-id="a0a14-146">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0a14-147">version</span><span class="sxs-lookup"><span data-stu-id="a0a14-147">version</span></span>|<span data-ttu-id="a0a14-148">String</span><span class="sxs-lookup"><span data-stu-id="a0a14-148">String</span></span>|<span data-ttu-id="a0a14-149">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="a0a14-149">Version of the entity.</span></span> <span data-ttu-id="a0a14-150">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0a14-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a0a14-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="a0a14-151">customSettings</span></span>|<span data-ttu-id="a0a14-152">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a0a14-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a0a14-153">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="a0a14-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0a14-154">Связи</span><span class="sxs-lookup"><span data-stu-id="a0a14-154">Relationships</span></span>
<span data-ttu-id="a0a14-155">Нет</span><span class="sxs-lookup"><span data-stu-id="a0a14-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0a14-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0a14-156">JSON Representation</span></span>
<span data-ttu-id="a0a14-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0a14-157">Here is a JSON representation of the resource.</span></span>
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




