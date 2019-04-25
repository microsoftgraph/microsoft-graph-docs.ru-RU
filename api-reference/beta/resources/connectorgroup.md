---
title: Тип ресурса Коннекторграуп
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543394"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="cc61a-103">Тип ресурса Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cc61a-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="cc61a-104">Методы</span><span class="sxs-lookup"><span data-stu-id="cc61a-104">Methods</span></span>

| <span data-ttu-id="cc61a-105">Метод</span><span class="sxs-lookup"><span data-stu-id="cc61a-105">Method</span></span>           | <span data-ttu-id="cc61a-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc61a-106">Return Type</span></span>    |<span data-ttu-id="cc61a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="cc61a-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc61a-108">Получение Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cc61a-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="cc61a-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="cc61a-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="cc61a-110">Чтение свойств и связей объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="cc61a-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="cc61a-111">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="cc61a-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="cc61a-112">application</span><span class="sxs-lookup"><span data-stu-id="cc61a-112">application</span></span>](application.md)| <span data-ttu-id="cc61a-113">Свяжите приложение с группой соединителей, размещая в коллекции Applications.</span><span class="sxs-lookup"><span data-stu-id="cc61a-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="cc61a-114">Перечисление приложений</span><span class="sxs-lookup"><span data-stu-id="cc61a-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="cc61a-115">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="cc61a-115">[application](application.md) collection</span></span>| <span data-ttu-id="cc61a-116">Получение связанной коллекции объектов Application.</span><span class="sxs-lookup"><span data-stu-id="cc61a-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="cc61a-117">Создание соединителя</span><span class="sxs-lookup"><span data-stu-id="cc61a-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="cc61a-118">PDIF</span><span class="sxs-lookup"><span data-stu-id="cc61a-118">connector</span></span>](connector.md)| <span data-ttu-id="cc61a-119">Добавьте соединитель в группу соединителей, отправив его в коллекцию Members.</span><span class="sxs-lookup"><span data-stu-id="cc61a-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="cc61a-120">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="cc61a-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="cc61a-121">[](connector.md) Коллекция соединителей</span><span class="sxs-lookup"><span data-stu-id="cc61a-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="cc61a-122">Получение коллекции объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="cc61a-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="cc61a-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="cc61a-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="cc61a-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="cc61a-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="cc61a-125">Обновление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="cc61a-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="cc61a-126">Удаление</span><span class="sxs-lookup"><span data-stu-id="cc61a-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="cc61a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="cc61a-127">None</span></span> |<span data-ttu-id="cc61a-128">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="cc61a-128">Delete connectorGroup object.</span></span> <span data-ttu-id="cc61a-129">Перед удалением группы конектор необходимо удалить все соединители.</span><span class="sxs-lookup"><span data-stu-id="cc61a-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc61a-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc61a-130">Properties</span></span>
| <span data-ttu-id="cc61a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc61a-131">Property</span></span>     | <span data-ttu-id="cc61a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cc61a-132">Type</span></span>   |<span data-ttu-id="cc61a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cc61a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc61a-134">Коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="cc61a-134">connectorGroupType</span></span>|<span data-ttu-id="cc61a-135">string</span><span class="sxs-lookup"><span data-stu-id="cc61a-135">string</span></span>| <span data-ttu-id="cc61a-136">Тип соединителей, которые будут использоваться для группы.</span><span class="sxs-lookup"><span data-stu-id="cc61a-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="cc61a-137">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="cc61a-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="cc61a-138">id</span><span class="sxs-lookup"><span data-stu-id="cc61a-138">id</span></span>|<span data-ttu-id="cc61a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="cc61a-139">String</span></span>| <span data-ttu-id="cc61a-140">Идентификатор объекта Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cc61a-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="cc61a-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="cc61a-141">isDefault</span></span>|<span data-ttu-id="cc61a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc61a-142">Boolean</span></span>| <span data-ttu-id="cc61a-143">Указывает, является ли Коннекторграуп группой соединителей по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cc61a-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="cc61a-144">Только одна группа соединителей может быть Коннекторграуп по умолчанию и задается системой.</span><span class="sxs-lookup"><span data-stu-id="cc61a-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="cc61a-145">name</span><span class="sxs-lookup"><span data-stu-id="cc61a-145">name</span></span>|<span data-ttu-id="cc61a-146">String</span><span class="sxs-lookup"><span data-stu-id="cc61a-146">String</span></span>| <span data-ttu-id="cc61a-147">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="cc61a-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc61a-148">Связи</span><span class="sxs-lookup"><span data-stu-id="cc61a-148">Relationships</span></span>
| <span data-ttu-id="cc61a-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="cc61a-149">Relationship</span></span> | <span data-ttu-id="cc61a-150">Тип</span><span class="sxs-lookup"><span data-stu-id="cc61a-150">Type</span></span>   |<span data-ttu-id="cc61a-151">Описание</span><span class="sxs-lookup"><span data-stu-id="cc61a-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc61a-152">заявлен</span><span class="sxs-lookup"><span data-stu-id="cc61a-152">applications</span></span>|<span data-ttu-id="cc61a-153">Коллекция [приложений](application.md)</span><span class="sxs-lookup"><span data-stu-id="cc61a-153">[application](application.md) collection</span></span>| <span data-ttu-id="cc61a-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc61a-154">Read-only.</span></span> <span data-ttu-id="cc61a-155">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="cc61a-155">Nullable.</span></span>|
|<span data-ttu-id="cc61a-156">members</span><span class="sxs-lookup"><span data-stu-id="cc61a-156">members</span></span>|<span data-ttu-id="cc61a-157">[](connector.md) Коллекция соединителей</span><span class="sxs-lookup"><span data-stu-id="cc61a-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="cc61a-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="cc61a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc61a-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cc61a-160">JSON representation</span></span>

<span data-ttu-id="cc61a-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc61a-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
