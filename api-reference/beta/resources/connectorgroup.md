---
title: Тип ресурса Коннекторграуп
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 5de46f480ff101e6d149bbfbe246ef47baff2604
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341204"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="0cc35-103">Тип ресурса Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="0cc35-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="0cc35-104">Методы</span><span class="sxs-lookup"><span data-stu-id="0cc35-104">Methods</span></span>

| <span data-ttu-id="0cc35-105">Метод</span><span class="sxs-lookup"><span data-stu-id="0cc35-105">Method</span></span>           | <span data-ttu-id="0cc35-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0cc35-106">Return Type</span></span>    |<span data-ttu-id="0cc35-107">Описание</span><span class="sxs-lookup"><span data-stu-id="0cc35-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cc35-108">Получение Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="0cc35-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="0cc35-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0cc35-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="0cc35-110">Чтение свойств и связей объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="0cc35-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="0cc35-111">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="0cc35-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="0cc35-112">application</span><span class="sxs-lookup"><span data-stu-id="0cc35-112">application</span></span>](application.md)| <span data-ttu-id="0cc35-113">Свяжите приложение с группой соединителей, размещая в коллекции Applications.</span><span class="sxs-lookup"><span data-stu-id="0cc35-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="0cc35-114">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="0cc35-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="0cc35-115">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="0cc35-115">[application](application.md) collection</span></span>| <span data-ttu-id="0cc35-116">Получение связанной коллекции объектов Application.</span><span class="sxs-lookup"><span data-stu-id="0cc35-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="0cc35-117">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="0cc35-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="0cc35-118">PDIF</span><span class="sxs-lookup"><span data-stu-id="0cc35-118">connector</span></span>](connector.md)| <span data-ttu-id="0cc35-119">Добавьте соединитель в группу соединителей, отправив его в коллекцию Members.</span><span class="sxs-lookup"><span data-stu-id="0cc35-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="0cc35-120">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="0cc35-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="0cc35-121">[](connector.md) Коллекция соединителей</span><span class="sxs-lookup"><span data-stu-id="0cc35-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="0cc35-122">Получение коллекции объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="0cc35-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="0cc35-123">Update</span><span class="sxs-lookup"><span data-stu-id="0cc35-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="0cc35-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0cc35-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="0cc35-125">Обновление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="0cc35-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="0cc35-126">Delete</span><span class="sxs-lookup"><span data-stu-id="0cc35-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="0cc35-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0cc35-127">None</span></span> |<span data-ttu-id="0cc35-128">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="0cc35-128">Delete connectorGroup object.</span></span> <span data-ttu-id="0cc35-129">Перед удалением группы конектор необходимо удалить все соединители.</span><span class="sxs-lookup"><span data-stu-id="0cc35-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="0cc35-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cc35-130">Properties</span></span>
| <span data-ttu-id="0cc35-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cc35-131">Property</span></span>     | <span data-ttu-id="0cc35-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0cc35-132">Type</span></span>   |<span data-ttu-id="0cc35-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0cc35-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cc35-134">Коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="0cc35-134">connectorGroupType</span></span>|<span data-ttu-id="0cc35-135">string</span><span class="sxs-lookup"><span data-stu-id="0cc35-135">string</span></span>| <span data-ttu-id="0cc35-136">Тип соединителей, которые будут использоваться для группы.</span><span class="sxs-lookup"><span data-stu-id="0cc35-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="0cc35-137">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="0cc35-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="0cc35-138">id</span><span class="sxs-lookup"><span data-stu-id="0cc35-138">id</span></span>|<span data-ttu-id="0cc35-139">Строка</span><span class="sxs-lookup"><span data-stu-id="0cc35-139">String</span></span>| <span data-ttu-id="0cc35-140">Идентификатор объекта Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="0cc35-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="0cc35-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="0cc35-141">isDefault</span></span>|<span data-ttu-id="0cc35-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cc35-142">Boolean</span></span>| <span data-ttu-id="0cc35-143">Указывает, является ли Коннекторграуп группой соединителей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0cc35-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="0cc35-144">Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.</span><span class="sxs-lookup"><span data-stu-id="0cc35-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="0cc35-145">name</span><span class="sxs-lookup"><span data-stu-id="0cc35-145">name</span></span>|<span data-ttu-id="0cc35-146">String</span><span class="sxs-lookup"><span data-stu-id="0cc35-146">String</span></span>| <span data-ttu-id="0cc35-147">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="0cc35-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cc35-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="0cc35-148">Relationships</span></span>
| <span data-ttu-id="0cc35-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="0cc35-149">Relationship</span></span> | <span data-ttu-id="0cc35-150">Тип</span><span class="sxs-lookup"><span data-stu-id="0cc35-150">Type</span></span>   |<span data-ttu-id="0cc35-151">Описание</span><span class="sxs-lookup"><span data-stu-id="0cc35-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cc35-152">заявлен</span><span class="sxs-lookup"><span data-stu-id="0cc35-152">applications</span></span>|<span data-ttu-id="0cc35-153">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="0cc35-153">[application](application.md) collection</span></span>| <span data-ttu-id="0cc35-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0cc35-154">Read-only.</span></span> <span data-ttu-id="0cc35-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0cc35-155">Nullable.</span></span>|
|<span data-ttu-id="0cc35-156">members</span><span class="sxs-lookup"><span data-stu-id="0cc35-156">members</span></span>|<span data-ttu-id="0cc35-157">[](connector.md) Коллекция соединителей</span><span class="sxs-lookup"><span data-stu-id="0cc35-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="0cc35-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0cc35-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cc35-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cc35-160">JSON representation</span></span>

<span data-ttu-id="0cc35-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cc35-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
