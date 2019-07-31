---
title: Тип ресурса Коннекторграуп
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d985f1f49ade4057b1a9ed9d3e1dbdafebfec7f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973207"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="c3281-103">Тип ресурса Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="c3281-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="c3281-104">Методы</span><span class="sxs-lookup"><span data-stu-id="c3281-104">Methods</span></span>

| <span data-ttu-id="c3281-105">Метод</span><span class="sxs-lookup"><span data-stu-id="c3281-105">Method</span></span>           | <span data-ttu-id="c3281-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3281-106">Return Type</span></span>    |<span data-ttu-id="c3281-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c3281-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3281-108">Получение Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="c3281-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="c3281-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="c3281-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="c3281-110">Чтение свойств и связей объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="c3281-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="c3281-111">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="c3281-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="c3281-112">application</span><span class="sxs-lookup"><span data-stu-id="c3281-112">application</span></span>](application.md)| <span data-ttu-id="c3281-113">Свяжите приложение с группой соединителей, размещая в коллекции Applications.</span><span class="sxs-lookup"><span data-stu-id="c3281-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="c3281-114">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="c3281-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="c3281-115">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="c3281-115">[application](application.md) collection</span></span>| <span data-ttu-id="c3281-116">Получение связанной коллекции объектов Application.</span><span class="sxs-lookup"><span data-stu-id="c3281-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="c3281-117">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="c3281-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="c3281-118">PDIF</span><span class="sxs-lookup"><span data-stu-id="c3281-118">connector</span></span>](connector.md)| <span data-ttu-id="c3281-119">Добавьте соединитель в группу соединителей, отправив его в коллекцию Members.</span><span class="sxs-lookup"><span data-stu-id="c3281-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="c3281-120">Список членов</span><span class="sxs-lookup"><span data-stu-id="c3281-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="c3281-121">[](connector.md) Коллекция соединителей</span><span class="sxs-lookup"><span data-stu-id="c3281-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="c3281-122">Получение коллекции объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="c3281-122">Get a connector object collection.</span></span>|
|<span data-ttu-id="c3281-123">[обновление](../api/connectorgroup-update.md);</span><span class="sxs-lookup"><span data-stu-id="c3281-123">[Update](../api/connectorgroup-update.md)</span></span> | [<span data-ttu-id="c3281-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="c3281-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="c3281-125">Обновление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="c3281-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="c3281-126">Удаление</span><span class="sxs-lookup"><span data-stu-id="c3281-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="c3281-127">Нет</span><span class="sxs-lookup"><span data-stu-id="c3281-127">None</span></span> |<span data-ttu-id="c3281-128">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="c3281-128">Delete connectorGroup object.</span></span> <span data-ttu-id="c3281-129">Перед удалением группы конектор необходимо удалить все соединители.</span><span class="sxs-lookup"><span data-stu-id="c3281-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3281-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3281-130">Properties</span></span>
| <span data-ttu-id="c3281-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3281-131">Property</span></span>     | <span data-ttu-id="c3281-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c3281-132">Type</span></span>   |<span data-ttu-id="c3281-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c3281-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3281-134">Коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="c3281-134">connectorGroupType</span></span>|<span data-ttu-id="c3281-135">string</span><span class="sxs-lookup"><span data-stu-id="c3281-135">string</span></span>| <span data-ttu-id="c3281-136">Тип соединителей, которые будут использоваться для группы.</span><span class="sxs-lookup"><span data-stu-id="c3281-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="c3281-137">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="c3281-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="c3281-138">id</span><span class="sxs-lookup"><span data-stu-id="c3281-138">id</span></span>|<span data-ttu-id="c3281-139">Строка</span><span class="sxs-lookup"><span data-stu-id="c3281-139">String</span></span>| <span data-ttu-id="c3281-140">Идентификатор объекта Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="c3281-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="c3281-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="c3281-141">isDefault</span></span>|<span data-ttu-id="c3281-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3281-142">Boolean</span></span>| <span data-ttu-id="c3281-143">Указывает, является ли Коннекторграуп группой соединителей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c3281-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="c3281-144">Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.</span><span class="sxs-lookup"><span data-stu-id="c3281-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="c3281-145">name</span><span class="sxs-lookup"><span data-stu-id="c3281-145">name</span></span>|<span data-ttu-id="c3281-146">String</span><span class="sxs-lookup"><span data-stu-id="c3281-146">String</span></span>| <span data-ttu-id="c3281-147">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="c3281-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3281-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="c3281-148">Relationships</span></span>
| <span data-ttu-id="c3281-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="c3281-149">Relationship</span></span> | <span data-ttu-id="c3281-150">Тип</span><span class="sxs-lookup"><span data-stu-id="c3281-150">Type</span></span>   |<span data-ttu-id="c3281-151">Описание</span><span class="sxs-lookup"><span data-stu-id="c3281-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3281-152">заявлен</span><span class="sxs-lookup"><span data-stu-id="c3281-152">applications</span></span>|<span data-ttu-id="c3281-153">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="c3281-153">[application](application.md) collection</span></span>| <span data-ttu-id="c3281-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3281-154">Read-only.</span></span> <span data-ttu-id="c3281-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c3281-155">Nullable.</span></span>|
|<span data-ttu-id="c3281-156">members</span><span class="sxs-lookup"><span data-stu-id="c3281-156">members</span></span>|<span data-ttu-id="c3281-157">[](connector.md) Коллекция соединителей</span><span class="sxs-lookup"><span data-stu-id="c3281-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="c3281-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c3281-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3281-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3281-160">JSON representation</span></span>

<span data-ttu-id="c3281-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3281-161">Here is a JSON representation of the resource.</span></span>

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
