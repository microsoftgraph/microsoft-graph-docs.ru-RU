---
title: тип ресурса printConnector
description: Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: e791ca755b695fc8e4704b65aff98a9db934d901
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517949"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="14f8f-104">тип ресурса printConnector</span><span class="sxs-lookup"><span data-stu-id="14f8f-104">printConnector resource type</span></span>

<span data-ttu-id="14f8f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14f8f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="14f8f-106">Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="14f8f-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="14f8f-107">Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.</span><span class="sxs-lookup"><span data-stu-id="14f8f-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="14f8f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="14f8f-108">Methods</span></span>
|<span data-ttu-id="14f8f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="14f8f-109">Method</span></span>|<span data-ttu-id="14f8f-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="14f8f-110">Return type</span></span>|<span data-ttu-id="14f8f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="14f8f-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="14f8f-112">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="14f8f-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="14f8f-113">printConnector</span><span class="sxs-lookup"><span data-stu-id="14f8f-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="14f8f-114">Ознакомьтесь с свойствами и отношениями объекта соединители.</span><span class="sxs-lookup"><span data-stu-id="14f8f-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="14f8f-115">Соединители обновления</span><span class="sxs-lookup"><span data-stu-id="14f8f-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="14f8f-116">printConnector</span><span class="sxs-lookup"><span data-stu-id="14f8f-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="14f8f-117">Обновление объекта соединители.</span><span class="sxs-lookup"><span data-stu-id="14f8f-117">Update the connector object.</span></span> |
| [<span data-ttu-id="14f8f-118">Удаление соединителя</span><span class="sxs-lookup"><span data-stu-id="14f8f-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="14f8f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="14f8f-119">None</span></span> | <span data-ttu-id="14f8f-120">Unregister the connector from the Universal Print service.</span><span class="sxs-lookup"><span data-stu-id="14f8f-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="14f8f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="14f8f-121">Properties</span></span>
|<span data-ttu-id="14f8f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="14f8f-122">Property</span></span>|<span data-ttu-id="14f8f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="14f8f-123">Type</span></span>|<span data-ttu-id="14f8f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="14f8f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14f8f-125">id</span><span class="sxs-lookup"><span data-stu-id="14f8f-125">id</span></span>|<span data-ttu-id="14f8f-126">String</span><span class="sxs-lookup"><span data-stu-id="14f8f-126">String</span></span>| <span data-ttu-id="14f8f-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14f8f-127">Read-only.</span></span>|
|<span data-ttu-id="14f8f-128">displayName</span><span class="sxs-lookup"><span data-stu-id="14f8f-128">displayName</span></span>|<span data-ttu-id="14f8f-129">Строка</span><span class="sxs-lookup"><span data-stu-id="14f8f-129">String</span></span>|<span data-ttu-id="14f8f-130">Имя соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="14f8f-130">The name of the connector.</span></span>|
|<span data-ttu-id="14f8f-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="14f8f-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="14f8f-132">Строка</span><span class="sxs-lookup"><span data-stu-id="14f8f-132">String</span></span>|<span data-ttu-id="14f8f-133">Имя хост-имени соединители.</span><span class="sxs-lookup"><span data-stu-id="14f8f-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="14f8f-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="14f8f-134">operatingSystem</span></span>|<span data-ttu-id="14f8f-135">String</span><span class="sxs-lookup"><span data-stu-id="14f8f-135">String</span></span>|<span data-ttu-id="14f8f-136">Версия операционной системы соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="14f8f-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="14f8f-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="14f8f-137">appVersion</span></span>|<span data-ttu-id="14f8f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="14f8f-138">String</span></span>|<span data-ttu-id="14f8f-139">Версия соединиттеля.</span><span class="sxs-lookup"><span data-stu-id="14f8f-139">The connector's version.</span></span>|
|<span data-ttu-id="14f8f-140">location</span><span class="sxs-lookup"><span data-stu-id="14f8f-140">location</span></span>|[<span data-ttu-id="14f8f-141">printerLocation</span><span class="sxs-lookup"><span data-stu-id="14f8f-141">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="14f8f-142">Физическое и/или организационное расположение соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="14f8f-142">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="14f8f-143">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="14f8f-143">registeredDateTime</span></span>|<span data-ttu-id="14f8f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14f8f-144">DateTimeOffset</span></span>|<span data-ttu-id="14f8f-145">DateTimeOffset при регистрации соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="14f8f-145">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="14f8f-146">registeredBy</span><span class="sxs-lookup"><span data-stu-id="14f8f-146">registeredBy</span></span>|[<span data-ttu-id="14f8f-147">userIdentity</span><span class="sxs-lookup"><span data-stu-id="14f8f-147">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="14f8f-148">Пользователь, зарегистрировавший соединители.</span><span class="sxs-lookup"><span data-stu-id="14f8f-148">The user who registered the connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14f8f-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="14f8f-149">Relationships</span></span>
<span data-ttu-id="14f8f-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14f8f-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14f8f-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14f8f-151">JSON representation</span></span>
<span data-ttu-id="14f8f-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14f8f-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```