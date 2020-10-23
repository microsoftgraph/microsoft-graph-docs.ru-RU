---
title: Тип ресурса Принтконнектор
description: Представляет соединитель печати, зарегистрированный с помощью универсальной подписки на печать. Ресурс Принтконнектор можно использовать для просмотра состояния соединителя и свойств обновления.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9962bad290d6a07c214107e58c8a96afb9148394
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727992"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="c64ee-104">Тип ресурса Принтконнектор</span><span class="sxs-lookup"><span data-stu-id="c64ee-104">printConnector resource type</span></span>

<span data-ttu-id="c64ee-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c64ee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c64ee-106">Представляет соединитель печати, зарегистрированный с помощью универсальной подписки на печать.</span><span class="sxs-lookup"><span data-stu-id="c64ee-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="c64ee-107">Ресурс Принтконнектор можно использовать для просмотра состояния соединителя и свойств обновления.</span><span class="sxs-lookup"><span data-stu-id="c64ee-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="c64ee-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c64ee-108">Methods</span></span>

| <span data-ttu-id="c64ee-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c64ee-109">Method</span></span>       | <span data-ttu-id="c64ee-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c64ee-110">Return Type</span></span> | <span data-ttu-id="c64ee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c64ee-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c64ee-112">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="c64ee-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="c64ee-113">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="c64ee-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="c64ee-114">Считывание свойств и связей объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="c64ee-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="c64ee-115">Соединитель обновления</span><span class="sxs-lookup"><span data-stu-id="c64ee-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="c64ee-116">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="c64ee-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="c64ee-117">Обновление объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="c64ee-117">Update the connector object.</span></span> |
| [<span data-ttu-id="c64ee-118">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="c64ee-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="c64ee-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c64ee-119">None</span></span> | <span data-ttu-id="c64ee-120">Отмените регистрацию соединителя в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="c64ee-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="c64ee-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c64ee-121">Properties</span></span>
| <span data-ttu-id="c64ee-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c64ee-122">Property</span></span>     | <span data-ttu-id="c64ee-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c64ee-123">Type</span></span>        | <span data-ttu-id="c64ee-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c64ee-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c64ee-125">id</span><span class="sxs-lookup"><span data-stu-id="c64ee-125">id</span></span>|<span data-ttu-id="c64ee-126">String</span><span class="sxs-lookup"><span data-stu-id="c64ee-126">String</span></span>| <span data-ttu-id="c64ee-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c64ee-127">Read-only.</span></span>|
|<span data-ttu-id="c64ee-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c64ee-128">displayName</span></span>|<span data-ttu-id="c64ee-129">Строка</span><span class="sxs-lookup"><span data-stu-id="c64ee-129">String</span></span>|<span data-ttu-id="c64ee-130">Имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="c64ee-130">The name of the connector.</span></span>|
|<span data-ttu-id="c64ee-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="c64ee-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="c64ee-132">Строка</span><span class="sxs-lookup"><span data-stu-id="c64ee-132">String</span></span>|<span data-ttu-id="c64ee-133">Имя узла для соединителя.</span><span class="sxs-lookup"><span data-stu-id="c64ee-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="c64ee-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c64ee-134">operatingSystem</span></span>|<span data-ttu-id="c64ee-135">String</span><span class="sxs-lookup"><span data-stu-id="c64ee-135">String</span></span>|<span data-ttu-id="c64ee-136">Версия операционной системы на соединителе компьютера.</span><span class="sxs-lookup"><span data-stu-id="c64ee-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="c64ee-137">аппверсион</span><span class="sxs-lookup"><span data-stu-id="c64ee-137">appVersion</span></span>|<span data-ttu-id="c64ee-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c64ee-138">String</span></span>|<span data-ttu-id="c64ee-139">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="c64ee-139">The connector's version.</span></span>|
|<span data-ttu-id="c64ee-140">девицехеалс</span><span class="sxs-lookup"><span data-stu-id="c64ee-140">deviceHealth</span></span>|[<span data-ttu-id="c64ee-141">девицехеалс</span><span class="sxs-lookup"><span data-stu-id="c64ee-141">deviceHealth</span></span>](devicehealth.md)|<span data-ttu-id="c64ee-142">Работоспособность устройства соединителя.</span><span class="sxs-lookup"><span data-stu-id="c64ee-142">The connector's device health.</span></span>|
|<span data-ttu-id="c64ee-143">location</span><span class="sxs-lookup"><span data-stu-id="c64ee-143">location</span></span>|[<span data-ttu-id="c64ee-144">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="c64ee-144">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="c64ee-145">Физическое и/или организационное расположение соединителя.</span><span class="sxs-lookup"><span data-stu-id="c64ee-145">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="c64ee-146">регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="c64ee-146">registeredDateTime</span></span>|<span data-ttu-id="c64ee-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c64ee-147">DateTimeOffset</span></span>|<span data-ttu-id="c64ee-148">Значение DateTimeOffset, когда соединитель был зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="c64ee-148">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="c64ee-149">регистередби</span><span class="sxs-lookup"><span data-stu-id="c64ee-149">registeredBy</span></span>|[<span data-ttu-id="c64ee-150">userIdentity</span><span class="sxs-lookup"><span data-stu-id="c64ee-150">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="c64ee-151">Пользователь, который зарегистрировал соединитель.</span><span class="sxs-lookup"><span data-stu-id="c64ee-151">The user who registered the connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c64ee-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c64ee-152">JSON representation</span></span>

<span data-ttu-id="c64ee-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c64ee-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


