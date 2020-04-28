---
title: Тип ресурса Коннекторграуп
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d57f116adac652cb55a3a270383ddb5c65d8e40f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507473"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="db36a-103">Тип ресурса Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="db36a-103">connectorGroup resource type</span></span>

<span data-ttu-id="db36a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db36a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="db36a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="db36a-105">Methods</span></span>

| <span data-ttu-id="db36a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="db36a-106">Method</span></span>           | <span data-ttu-id="db36a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="db36a-107">Return Type</span></span>    |<span data-ttu-id="db36a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="db36a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db36a-109">Получение Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="db36a-109">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="db36a-110">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="db36a-110">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="db36a-111">Чтение свойств и связей объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="db36a-111">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="db36a-112">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="db36a-112">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="db36a-113">application</span><span class="sxs-lookup"><span data-stu-id="db36a-113">application</span></span>](application.md)| <span data-ttu-id="db36a-114">Свяжите приложение с группой соединителей, размещая в коллекции Applications.</span><span class="sxs-lookup"><span data-stu-id="db36a-114">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="db36a-115">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="db36a-115">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="db36a-116">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-116">[application](application.md) collection</span></span>| <span data-ttu-id="db36a-117">Получение связанной коллекции объектов Application.</span><span class="sxs-lookup"><span data-stu-id="db36a-117">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="db36a-118">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="db36a-118">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="db36a-119">PDIF</span><span class="sxs-lookup"><span data-stu-id="db36a-119">connector</span></span>](connector.md)| <span data-ttu-id="db36a-120">Добавьте соединитель в группу соединителей, отправив его в коллекцию Members.</span><span class="sxs-lookup"><span data-stu-id="db36a-120">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="db36a-121">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="db36a-121">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="db36a-122">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-122">[connector](connector.md) collection</span></span>| <span data-ttu-id="db36a-123">Получение коллекции объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="db36a-123">Get a connector object collection.</span></span>|
|<span data-ttu-id="db36a-124">[обновление](../api/connectorgroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="db36a-124">[Update](../api/connectorgroup-update.md)</span></span> | [<span data-ttu-id="db36a-125">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="db36a-125">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="db36a-126">Обновление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="db36a-126">Update connectorGroup object.</span></span> |
|<span data-ttu-id="db36a-127">[удаление](../api/connectorgroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="db36a-127">[Delete](../api/connectorgroup-delete.md)</span></span> | <span data-ttu-id="db36a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="db36a-128">None</span></span> |<span data-ttu-id="db36a-129">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="db36a-129">Delete connectorGroup object.</span></span> <span data-ttu-id="db36a-130">Перед удалением группы соединителей необходимо удалить все соединители.</span><span class="sxs-lookup"><span data-stu-id="db36a-130">All connectors must be remove before a connector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="db36a-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="db36a-131">Properties</span></span>
| <span data-ttu-id="db36a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="db36a-132">Property</span></span>     | <span data-ttu-id="db36a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="db36a-133">Type</span></span>   |<span data-ttu-id="db36a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="db36a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db36a-135">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="db36a-135">connectorGroupType</span></span>|<span data-ttu-id="db36a-136">string</span><span class="sxs-lookup"><span data-stu-id="db36a-136">string</span></span>| <span data-ttu-id="db36a-137">Тип соединителей, которые будут использоваться для группы.</span><span class="sxs-lookup"><span data-stu-id="db36a-137">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="db36a-138">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="db36a-138">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="db36a-139">id</span><span class="sxs-lookup"><span data-stu-id="db36a-139">id</span></span>|<span data-ttu-id="db36a-140">Строка</span><span class="sxs-lookup"><span data-stu-id="db36a-140">String</span></span>| <span data-ttu-id="db36a-141">Идентификатор объекта Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="db36a-141">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="db36a-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="db36a-142">isDefault</span></span>|<span data-ttu-id="db36a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="db36a-143">Boolean</span></span>| <span data-ttu-id="db36a-144">Указывает, является ли Коннекторграуп группой соединителей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="db36a-144">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="db36a-145">Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.</span><span class="sxs-lookup"><span data-stu-id="db36a-145">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="db36a-146">name</span><span class="sxs-lookup"><span data-stu-id="db36a-146">name</span></span>|<span data-ttu-id="db36a-147">String</span><span class="sxs-lookup"><span data-stu-id="db36a-147">String</span></span>| <span data-ttu-id="db36a-148">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="db36a-148">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db36a-149">Связи</span><span class="sxs-lookup"><span data-stu-id="db36a-149">Relationships</span></span>
| <span data-ttu-id="db36a-150">Связь</span><span class="sxs-lookup"><span data-stu-id="db36a-150">Relationship</span></span> | <span data-ttu-id="db36a-151">Тип</span><span class="sxs-lookup"><span data-stu-id="db36a-151">Type</span></span>   |<span data-ttu-id="db36a-152">Описание</span><span class="sxs-lookup"><span data-stu-id="db36a-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db36a-153">заявлен</span><span class="sxs-lookup"><span data-stu-id="db36a-153">applications</span></span>|<span data-ttu-id="db36a-154">Коллекция [application](application.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-154">[application](application.md) collection</span></span>| <span data-ttu-id="db36a-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db36a-155">Read-only.</span></span> <span data-ttu-id="db36a-156">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="db36a-156">Nullable.</span></span>|
|<span data-ttu-id="db36a-157">members</span><span class="sxs-lookup"><span data-stu-id="db36a-157">members</span></span>|<span data-ttu-id="db36a-158">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="db36a-158">[connector](connector.md) collection</span></span>| <span data-ttu-id="db36a-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="db36a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db36a-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db36a-161">JSON representation</span></span>

<span data-ttu-id="db36a-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db36a-162">Here is a JSON representation of the resource.</span></span>

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
