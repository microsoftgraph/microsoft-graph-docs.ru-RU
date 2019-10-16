---
title: Тип ресурса Коннекторграуп
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 02ef418f0f2124b4bd0c7489db8c732398005761
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538387"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="f54e2-103">Тип ресурса Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="f54e2-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="f54e2-104">Методы</span><span class="sxs-lookup"><span data-stu-id="f54e2-104">Methods</span></span>

| <span data-ttu-id="f54e2-105">Метод</span><span class="sxs-lookup"><span data-stu-id="f54e2-105">Method</span></span>           | <span data-ttu-id="f54e2-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f54e2-106">Return Type</span></span>    |<span data-ttu-id="f54e2-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f54e2-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f54e2-108">Получение Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="f54e2-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="f54e2-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f54e2-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="f54e2-110">Чтение свойств и связей объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="f54e2-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="f54e2-111">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="f54e2-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="f54e2-112">application</span><span class="sxs-lookup"><span data-stu-id="f54e2-112">application</span></span>](application.md)| <span data-ttu-id="f54e2-113">Свяжите приложение с группой соединителей, размещая в коллекции Applications.</span><span class="sxs-lookup"><span data-stu-id="f54e2-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="f54e2-114">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="f54e2-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="f54e2-115">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="f54e2-115">[application](application.md) collection</span></span>| <span data-ttu-id="f54e2-116">Получение связанной коллекции объектов Application.</span><span class="sxs-lookup"><span data-stu-id="f54e2-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="f54e2-117">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="f54e2-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="f54e2-118">PDIF</span><span class="sxs-lookup"><span data-stu-id="f54e2-118">connector</span></span>](connector.md)| <span data-ttu-id="f54e2-119">Добавьте соединитель в группу соединителей, отправив его в коллекцию Members.</span><span class="sxs-lookup"><span data-stu-id="f54e2-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="f54e2-120">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="f54e2-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="f54e2-121">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="f54e2-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="f54e2-122">Получение коллекции объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="f54e2-122">Get a connector object collection.</span></span>|
|<span data-ttu-id="f54e2-123">[обновление](../api/connectorgroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="f54e2-123">[Update](../api/connectorgroup-update.md)</span></span> | [<span data-ttu-id="f54e2-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f54e2-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="f54e2-125">Обновление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="f54e2-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="f54e2-126">Удаление</span><span class="sxs-lookup"><span data-stu-id="f54e2-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="f54e2-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f54e2-127">None</span></span> |<span data-ttu-id="f54e2-128">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="f54e2-128">Delete connectorGroup object.</span></span> <span data-ttu-id="f54e2-129">Перед удалением группы соединителей необходимо удалить все соединители.</span><span class="sxs-lookup"><span data-stu-id="f54e2-129">All connectors must be remove before a connector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="f54e2-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="f54e2-130">Properties</span></span>
| <span data-ttu-id="f54e2-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f54e2-131">Property</span></span>     | <span data-ttu-id="f54e2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f54e2-132">Type</span></span>   |<span data-ttu-id="f54e2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f54e2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f54e2-134">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="f54e2-134">connectorGroupType</span></span>|<span data-ttu-id="f54e2-135">string</span><span class="sxs-lookup"><span data-stu-id="f54e2-135">string</span></span>| <span data-ttu-id="f54e2-136">Тип соединителей, которые будут использоваться для группы.</span><span class="sxs-lookup"><span data-stu-id="f54e2-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="f54e2-137">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="f54e2-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="f54e2-138">id</span><span class="sxs-lookup"><span data-stu-id="f54e2-138">id</span></span>|<span data-ttu-id="f54e2-139">Строка</span><span class="sxs-lookup"><span data-stu-id="f54e2-139">String</span></span>| <span data-ttu-id="f54e2-140">Идентификатор объекта Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="f54e2-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="f54e2-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="f54e2-141">isDefault</span></span>|<span data-ttu-id="f54e2-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f54e2-142">Boolean</span></span>| <span data-ttu-id="f54e2-143">Указывает, является ли Коннекторграуп группой соединителей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f54e2-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="f54e2-144">Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.</span><span class="sxs-lookup"><span data-stu-id="f54e2-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="f54e2-145">name</span><span class="sxs-lookup"><span data-stu-id="f54e2-145">name</span></span>|<span data-ttu-id="f54e2-146">String</span><span class="sxs-lookup"><span data-stu-id="f54e2-146">String</span></span>| <span data-ttu-id="f54e2-147">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="f54e2-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f54e2-148">Связи</span><span class="sxs-lookup"><span data-stu-id="f54e2-148">Relationships</span></span>
| <span data-ttu-id="f54e2-149">Связь</span><span class="sxs-lookup"><span data-stu-id="f54e2-149">Relationship</span></span> | <span data-ttu-id="f54e2-150">Тип</span><span class="sxs-lookup"><span data-stu-id="f54e2-150">Type</span></span>   |<span data-ttu-id="f54e2-151">Описание</span><span class="sxs-lookup"><span data-stu-id="f54e2-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f54e2-152">заявлен</span><span class="sxs-lookup"><span data-stu-id="f54e2-152">applications</span></span>|<span data-ttu-id="f54e2-153">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="f54e2-153">[application](application.md) collection</span></span>| <span data-ttu-id="f54e2-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f54e2-154">Read-only.</span></span> <span data-ttu-id="f54e2-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f54e2-155">Nullable.</span></span>|
|<span data-ttu-id="f54e2-156">members</span><span class="sxs-lookup"><span data-stu-id="f54e2-156">members</span></span>|<span data-ttu-id="f54e2-157">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="f54e2-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="f54e2-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f54e2-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f54e2-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f54e2-160">JSON representation</span></span>

<span data-ttu-id="f54e2-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f54e2-161">Here is a JSON representation of the resource.</span></span>

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
