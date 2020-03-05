---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60ee8156773db386d5ad8496bf037984005dc5bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448433"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="71847-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="71847-103">managedAppConfiguration resource type</span></span>

<span data-ttu-id="71847-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="71847-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71847-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71847-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71847-106">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="71847-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="71847-107">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="71847-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="71847-108">Методы</span><span class="sxs-lookup"><span data-stu-id="71847-108">Methods</span></span>
|<span data-ttu-id="71847-109">Метод</span><span class="sxs-lookup"><span data-stu-id="71847-109">Method</span></span>|<span data-ttu-id="71847-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="71847-110">Return Type</span></span>|<span data-ttu-id="71847-111">Описание</span><span class="sxs-lookup"><span data-stu-id="71847-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71847-112">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="71847-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="71847-113">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71847-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="71847-114">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71847-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="71847-115">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="71847-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="71847-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="71847-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="71847-117">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71847-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71847-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="71847-118">Properties</span></span>
|<span data-ttu-id="71847-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="71847-119">Property</span></span>|<span data-ttu-id="71847-120">Тип</span><span class="sxs-lookup"><span data-stu-id="71847-120">Type</span></span>|<span data-ttu-id="71847-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71847-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71847-122">displayName</span><span class="sxs-lookup"><span data-stu-id="71847-122">displayName</span></span>|<span data-ttu-id="71847-123">Строка</span><span class="sxs-lookup"><span data-stu-id="71847-123">String</span></span>|<span data-ttu-id="71847-124">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="71847-124">Policy display name.</span></span> <span data-ttu-id="71847-125">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71847-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="71847-126">description</span><span class="sxs-lookup"><span data-stu-id="71847-126">description</span></span>|<span data-ttu-id="71847-127">String</span><span class="sxs-lookup"><span data-stu-id="71847-127">String</span></span>|<span data-ttu-id="71847-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="71847-128">The policy's description.</span></span> <span data-ttu-id="71847-129">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71847-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="71847-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71847-130">createdDateTime</span></span>|<span data-ttu-id="71847-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71847-131">DateTimeOffset</span></span>|<span data-ttu-id="71847-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="71847-132">The date and time the policy was created.</span></span> <span data-ttu-id="71847-133">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71847-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="71847-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71847-134">lastModifiedDateTime</span></span>|<span data-ttu-id="71847-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71847-135">DateTimeOffset</span></span>|<span data-ttu-id="71847-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="71847-136">Last time the policy was modified.</span></span> <span data-ttu-id="71847-137">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71847-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="71847-138">id</span><span class="sxs-lookup"><span data-stu-id="71847-138">id</span></span>|<span data-ttu-id="71847-139">String</span><span class="sxs-lookup"><span data-stu-id="71847-139">String</span></span>|<span data-ttu-id="71847-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71847-140">Key of the entity.</span></span> <span data-ttu-id="71847-141">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71847-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="71847-142">version</span><span class="sxs-lookup"><span data-stu-id="71847-142">version</span></span>|<span data-ttu-id="71847-143">String</span><span class="sxs-lookup"><span data-stu-id="71847-143">String</span></span>|<span data-ttu-id="71847-144">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="71847-144">Version of the entity.</span></span> <span data-ttu-id="71847-145">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71847-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="71847-146">customSettings</span><span class="sxs-lookup"><span data-stu-id="71847-146">customSettings</span></span>|<span data-ttu-id="71847-147">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="71847-147">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="71847-148">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="71847-148">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="71847-149">Связи</span><span class="sxs-lookup"><span data-stu-id="71847-149">Relationships</span></span>
<span data-ttu-id="71847-150">Нет</span><span class="sxs-lookup"><span data-stu-id="71847-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71847-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71847-151">JSON Representation</span></span>
<span data-ttu-id="71847-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71847-152">Here is a JSON representation of the resource.</span></span>
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




