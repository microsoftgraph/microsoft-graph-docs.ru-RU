---
title: Тип ресурса managedAppConfiguration
description: Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация
ms.openlocfilehash: 42544aeacda4494a7757a15bef75a493d96fe0cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028294"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="8c107-103">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c107-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="8c107-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c107-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c107-105">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="8c107-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="8c107-106">Наследуется от [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c107-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8c107-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8c107-107">Methods</span></span>
|<span data-ttu-id="8c107-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8c107-108">Method</span></span>|<span data-ttu-id="8c107-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c107-109">Return Type</span></span>|<span data-ttu-id="8c107-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c107-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c107-111">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8c107-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="8c107-112">Коллекция [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c107-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="8c107-113">Список свойств и связей объектов [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8c107-114">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c107-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="8c107-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c107-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="8c107-116">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c107-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c107-117">Properties</span></span>
|<span data-ttu-id="8c107-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c107-118">Property</span></span>|<span data-ttu-id="8c107-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8c107-119">Type</span></span>|<span data-ttu-id="8c107-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8c107-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c107-121">displayName</span><span class="sxs-lookup"><span data-stu-id="8c107-121">displayName</span></span>|<span data-ttu-id="8c107-122">String</span><span class="sxs-lookup"><span data-stu-id="8c107-122">String</span></span>|<span data-ttu-id="8c107-123">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="8c107-123">Policy display name.</span></span> <span data-ttu-id="8c107-124">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c107-125">описание</span><span class="sxs-lookup"><span data-stu-id="8c107-125">description</span></span>|<span data-ttu-id="8c107-126">String</span><span class="sxs-lookup"><span data-stu-id="8c107-126">String</span></span>|<span data-ttu-id="8c107-127">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="8c107-127">The policy's description.</span></span> <span data-ttu-id="8c107-128">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c107-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c107-129">createdDateTime</span></span>|<span data-ttu-id="8c107-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c107-130">DateTimeOffset</span></span>|<span data-ttu-id="8c107-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="8c107-131">The date and time the policy was created.</span></span> <span data-ttu-id="8c107-132">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c107-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c107-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8c107-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c107-134">DateTimeOffset</span></span>|<span data-ttu-id="8c107-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="8c107-135">Last time the policy was modified.</span></span> <span data-ttu-id="8c107-136">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c107-137">id</span><span class="sxs-lookup"><span data-stu-id="8c107-137">id</span></span>|<span data-ttu-id="8c107-138">String</span><span class="sxs-lookup"><span data-stu-id="8c107-138">String</span></span>|<span data-ttu-id="8c107-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8c107-139">Key of the entity.</span></span> <span data-ttu-id="8c107-140">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c107-141">version</span><span class="sxs-lookup"><span data-stu-id="8c107-141">version</span></span>|<span data-ttu-id="8c107-142">String</span><span class="sxs-lookup"><span data-stu-id="8c107-142">String</span></span>|<span data-ttu-id="8c107-143">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8c107-143">Version of the entity.</span></span> <span data-ttu-id="8c107-144">Наследуется от объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c107-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="8c107-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="8c107-145">customSettings</span></span>|<span data-ttu-id="8c107-146">Коллекция [keyValuePair](../resources/intune-mam-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8c107-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8c107-147">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="8c107-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c107-148">Связи</span><span class="sxs-lookup"><span data-stu-id="8c107-148">Relationships</span></span>
<span data-ttu-id="8c107-149">Нет</span><span class="sxs-lookup"><span data-stu-id="8c107-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c107-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c107-150">JSON Representation</span></span>
<span data-ttu-id="8c107-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c107-151">Here is a JSON representation of the resource.</span></span>
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



