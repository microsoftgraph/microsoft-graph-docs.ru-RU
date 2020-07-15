---
title: Тип ресурса Принтконнектор
description: Представляет соединитель печати, зарегистрированный с помощью универсальной подписки на печать. Ресурс Принтконнектор можно использовать для просмотра состояния соединителя и свойств обновления.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 84c9625bd8d5a454100cab166676c1dcbcfd8d05
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142430"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="f2416-104">Тип ресурса Принтконнектор</span><span class="sxs-lookup"><span data-stu-id="f2416-104">printConnector resource type</span></span>

<span data-ttu-id="f2416-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2416-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2416-106">Представляет соединитель печати, зарегистрированный с помощью универсальной подписки на печать.</span><span class="sxs-lookup"><span data-stu-id="f2416-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="f2416-107">Ресурс Принтконнектор можно использовать для просмотра состояния соединителя и свойств обновления.</span><span class="sxs-lookup"><span data-stu-id="f2416-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="f2416-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f2416-108">Methods</span></span>

| <span data-ttu-id="f2416-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f2416-109">Method</span></span>       | <span data-ttu-id="f2416-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2416-110">Return Type</span></span> | <span data-ttu-id="f2416-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f2416-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f2416-112">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="f2416-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="f2416-113">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="f2416-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="f2416-114">Считывание свойств и связей объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="f2416-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="f2416-115">Соединитель обновления</span><span class="sxs-lookup"><span data-stu-id="f2416-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="f2416-116">принтконнектор</span><span class="sxs-lookup"><span data-stu-id="f2416-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="f2416-117">Обновление объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="f2416-117">Update the connector object.</span></span> |
| [<span data-ttu-id="f2416-118">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="f2416-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="f2416-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f2416-119">None</span></span> | <span data-ttu-id="f2416-120">Отмените регистрацию соединителя в универсальной службе печати.</span><span class="sxs-lookup"><span data-stu-id="f2416-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2416-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2416-121">Properties</span></span>
| <span data-ttu-id="f2416-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2416-122">Property</span></span>     | <span data-ttu-id="f2416-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f2416-123">Type</span></span>        | <span data-ttu-id="f2416-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f2416-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2416-125">id</span><span class="sxs-lookup"><span data-stu-id="f2416-125">id</span></span>|<span data-ttu-id="f2416-126">String</span><span class="sxs-lookup"><span data-stu-id="f2416-126">String</span></span>| <span data-ttu-id="f2416-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2416-127">Read-only.</span></span>|
|<span data-ttu-id="f2416-128">name</span><span class="sxs-lookup"><span data-stu-id="f2416-128">name</span></span>|<span data-ttu-id="f2416-129">String</span><span class="sxs-lookup"><span data-stu-id="f2416-129">String</span></span>|<span data-ttu-id="f2416-130">Имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="f2416-130">The name of the connector.</span></span>|
|<span data-ttu-id="f2416-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="f2416-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="f2416-132">String</span><span class="sxs-lookup"><span data-stu-id="f2416-132">String</span></span>|<span data-ttu-id="f2416-133">Имя узла для соединителя.</span><span class="sxs-lookup"><span data-stu-id="f2416-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="f2416-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2416-134">operatingSystem</span></span>|<span data-ttu-id="f2416-135">String</span><span class="sxs-lookup"><span data-stu-id="f2416-135">String</span></span>|<span data-ttu-id="f2416-136">Версия операционной системы на соединителе компьютера.</span><span class="sxs-lookup"><span data-stu-id="f2416-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="f2416-137">аппверсион</span><span class="sxs-lookup"><span data-stu-id="f2416-137">appVersion</span></span>|<span data-ttu-id="f2416-138">String</span><span class="sxs-lookup"><span data-stu-id="f2416-138">String</span></span>|<span data-ttu-id="f2416-139">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="f2416-139">The connector's version.</span></span>|
|<span data-ttu-id="f2416-140">девицехеалс</span><span class="sxs-lookup"><span data-stu-id="f2416-140">deviceHealth</span></span>|[<span data-ttu-id="f2416-141">девицехеалс</span><span class="sxs-lookup"><span data-stu-id="f2416-141">deviceHealth</span></span>](devicehealth.md)|<span data-ttu-id="f2416-142">Работоспособность устройства соединителя.</span><span class="sxs-lookup"><span data-stu-id="f2416-142">The connector's device health.</span></span>|
|<span data-ttu-id="f2416-143">location</span><span class="sxs-lookup"><span data-stu-id="f2416-143">location</span></span>|[<span data-ttu-id="f2416-144">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="f2416-144">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="f2416-145">Физическое и/или организационное расположение соединителя.</span><span class="sxs-lookup"><span data-stu-id="f2416-145">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="f2416-146">регистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="f2416-146">registeredDateTime</span></span>|<span data-ttu-id="f2416-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2416-147">DateTimeOffset</span></span>|<span data-ttu-id="f2416-148">Значение DateTimeOffset, когда соединитель был зарегистрирован.</span><span class="sxs-lookup"><span data-stu-id="f2416-148">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="f2416-149">регистередби</span><span class="sxs-lookup"><span data-stu-id="f2416-149">registeredBy</span></span>|[<span data-ttu-id="f2416-150">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f2416-150">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="f2416-151">Пользователь, который зарегистрировал соединитель.</span><span class="sxs-lookup"><span data-stu-id="f2416-151">The user who registered the connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2416-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2416-152">JSON representation</span></span>

<span data-ttu-id="f2416-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2416-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
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
