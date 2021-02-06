---
title: Тип ресурса outlookCategory
description: Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. В Outlook пользователь определяет категории в этом списке и может применить одну или несколько из этих пользовательских категорий.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 516a4c42a93577b822f3b28ec1f0e886319905df
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130005"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="bd77b-104">Тип ресурса outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bd77b-104">outlookCategory resource type</span></span>

<span data-ttu-id="bd77b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd77b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="bd77b-106">Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события.</span><span class="sxs-lookup"><span data-stu-id="bd77b-106">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="bd77b-107">В Outlook пользователь определяет категории в этом списке и может применить к элементу одну или несколько из этих пользовательских категорий.</span><span class="sxs-lookup"><span data-stu-id="bd77b-107">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="bd77b-108">С помощью REST API вы можете [создавать](../api/outlookuser-post-mastercategories.md) и определять категории в основном списке категорий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd77b-108">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="bd77b-109">Вы также можете [получить этот основной список категорий](../api/outlookuser-list-mastercategories.md), [получить определенную категорию](../api/outlookcategory-get.md), [изменить](../api/outlookcategory-update.md) цвет, связанный с категорией, или [удалить](../api/outlookcategory-delete.md) категорию.</span><span class="sxs-lookup"><span data-stu-id="bd77b-109">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="bd77b-110">Вы можете применить категорию к списку, добавив значение свойства **displayName** категории в коллекцию **categories** элемента.</span><span class="sxs-lookup"><span data-stu-id="bd77b-110">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="bd77b-111">К ресурсам, которые могут быть назначены категориям, относятся [контакт,](contact.md) [событие,](event.md) [сообщение,](message.md) [outlookTask](outlooktask.md)и [публикация.](post.md)</span><span class="sxs-lookup"><span data-stu-id="bd77b-111">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="bd77b-112">Каждой категории назначается 2 свойства: **displayName** и **color**.</span><span class="sxs-lookup"><span data-stu-id="bd77b-112">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="bd77b-113">Значение **displayName** должно быть уникальным в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd77b-113">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="bd77b-114">Однако значение свойства **color** может не быть уникальным. Несколько категорий в основном списке можно сопоставить с одним цветом.</span><span class="sxs-lookup"><span data-stu-id="bd77b-114">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="bd77b-115">Вы можете сопоставить до 25 различных цветов с категориями в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd77b-115">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="bd77b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd77b-116">Properties</span></span>
| <span data-ttu-id="bd77b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd77b-117">Property</span></span>     | <span data-ttu-id="bd77b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="bd77b-118">Type</span></span>   |<span data-ttu-id="bd77b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bd77b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd77b-120">displayName</span><span class="sxs-lookup"><span data-stu-id="bd77b-120">displayName</span></span>|<span data-ttu-id="bd77b-121">Строка</span><span class="sxs-lookup"><span data-stu-id="bd77b-121">String</span></span>|<span data-ttu-id="bd77b-122">Уникальное имя, обозначающее категорию в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd77b-122">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="bd77b-123">После создания категории изменить имя невозможно.</span><span class="sxs-lookup"><span data-stu-id="bd77b-123">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="bd77b-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd77b-124">Read-only.</span></span>|
|<span data-ttu-id="bd77b-125">color</span><span class="sxs-lookup"><span data-stu-id="bd77b-125">color</span></span>|<span data-ttu-id="bd77b-126">String</span><span class="sxs-lookup"><span data-stu-id="bd77b-126">String</span></span>|<span data-ttu-id="bd77b-127">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="bd77b-127">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="bd77b-128">См. примечание ниже.</span><span class="sxs-lookup"><span data-stu-id="bd77b-128">See the note below.</span></span> |

> <span data-ttu-id="bd77b-129">**Примечание**. Допустимые значения свойства **color** — предустановленные константы, например `None`, `preset0` и `preset1`.</span><span class="sxs-lookup"><span data-stu-id="bd77b-129">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="bd77b-130">Каждая предустановленная константа сопоставлена с цветом. Фактический цвет зависит от клиента Outlook, в котором отображаются категории.</span><span class="sxs-lookup"><span data-stu-id="bd77b-130">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="bd77b-131">В приведенной ниже таблице показаны цвета, сопоставленные с каждой предустановленной константой для классического клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="bd77b-131">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="bd77b-132">Предустановленная константа</span><span class="sxs-lookup"><span data-stu-id="bd77b-132">Pre-set constant</span></span>  | <span data-ttu-id="bd77b-133">Соответствующий цвет в Outlook</span><span class="sxs-lookup"><span data-stu-id="bd77b-133">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd77b-134">None</span><span class="sxs-lookup"><span data-stu-id="bd77b-134">None</span></span> | <span data-ttu-id="bd77b-135">Цвет не задан</span><span class="sxs-lookup"><span data-stu-id="bd77b-135">No color mapped</span></span> |
| <span data-ttu-id="bd77b-136">Preset0</span><span class="sxs-lookup"><span data-stu-id="bd77b-136">Preset0</span></span> | <span data-ttu-id="bd77b-137">Красный</span><span class="sxs-lookup"><span data-stu-id="bd77b-137">Red</span></span> |
| <span data-ttu-id="bd77b-138">Preset1</span><span class="sxs-lookup"><span data-stu-id="bd77b-138">Preset1</span></span> | <span data-ttu-id="bd77b-139">Оранжевый</span><span class="sxs-lookup"><span data-stu-id="bd77b-139">Orange</span></span> |
| <span data-ttu-id="bd77b-140">Preset2</span><span class="sxs-lookup"><span data-stu-id="bd77b-140">Preset2</span></span> | <span data-ttu-id="bd77b-141">Коричневый</span><span class="sxs-lookup"><span data-stu-id="bd77b-141">Brown</span></span> |
| <span data-ttu-id="bd77b-142">Preset3</span><span class="sxs-lookup"><span data-stu-id="bd77b-142">Preset3</span></span> | <span data-ttu-id="bd77b-143">Желтый</span><span class="sxs-lookup"><span data-stu-id="bd77b-143">Yellow</span></span> |
| <span data-ttu-id="bd77b-144">Preset4</span><span class="sxs-lookup"><span data-stu-id="bd77b-144">Preset4</span></span> | <span data-ttu-id="bd77b-145">Зеленый</span><span class="sxs-lookup"><span data-stu-id="bd77b-145">Green</span></span> |
| <span data-ttu-id="bd77b-146">Preset5</span><span class="sxs-lookup"><span data-stu-id="bd77b-146">Preset5</span></span> | <span data-ttu-id="bd77b-147">Сине-зеленый</span><span class="sxs-lookup"><span data-stu-id="bd77b-147">Teal</span></span> |
| <span data-ttu-id="bd77b-148">Preset6</span><span class="sxs-lookup"><span data-stu-id="bd77b-148">Preset6</span></span> | <span data-ttu-id="bd77b-149">Оливковый</span><span class="sxs-lookup"><span data-stu-id="bd77b-149">Olive</span></span> |
| <span data-ttu-id="bd77b-150">Preset7</span><span class="sxs-lookup"><span data-stu-id="bd77b-150">Preset7</span></span> | <span data-ttu-id="bd77b-151">Синий</span><span class="sxs-lookup"><span data-stu-id="bd77b-151">Blue</span></span> |
| <span data-ttu-id="bd77b-152">Preset8</span><span class="sxs-lookup"><span data-stu-id="bd77b-152">Preset8</span></span> | <span data-ttu-id="bd77b-153">Сиреневый</span><span class="sxs-lookup"><span data-stu-id="bd77b-153">Purple</span></span> |
| <span data-ttu-id="bd77b-154">Preset9</span><span class="sxs-lookup"><span data-stu-id="bd77b-154">Preset9</span></span> | <span data-ttu-id="bd77b-155">Клюквенный</span><span class="sxs-lookup"><span data-stu-id="bd77b-155">Cranberry</span></span> |
| <span data-ttu-id="bd77b-156">Preset10</span><span class="sxs-lookup"><span data-stu-id="bd77b-156">Preset10</span></span> | <span data-ttu-id="bd77b-157">Стальной</span><span class="sxs-lookup"><span data-stu-id="bd77b-157">Steel</span></span> |
| <span data-ttu-id="bd77b-158">Preset11</span><span class="sxs-lookup"><span data-stu-id="bd77b-158">Preset11</span></span> | <span data-ttu-id="bd77b-159">Темно-стальной</span><span class="sxs-lookup"><span data-stu-id="bd77b-159">DarkSteel</span></span> |
| <span data-ttu-id="bd77b-160">Preset12</span><span class="sxs-lookup"><span data-stu-id="bd77b-160">Preset12</span></span> | <span data-ttu-id="bd77b-161">Серый</span><span class="sxs-lookup"><span data-stu-id="bd77b-161">Gray</span></span> |
| <span data-ttu-id="bd77b-162">Preset13</span><span class="sxs-lookup"><span data-stu-id="bd77b-162">Preset13</span></span> | <span data-ttu-id="bd77b-163">Темно-серый</span><span class="sxs-lookup"><span data-stu-id="bd77b-163">DarkGray</span></span> |
| <span data-ttu-id="bd77b-164">Preset14</span><span class="sxs-lookup"><span data-stu-id="bd77b-164">Preset14</span></span> | <span data-ttu-id="bd77b-165">Черный</span><span class="sxs-lookup"><span data-stu-id="bd77b-165">Black</span></span> |
| <span data-ttu-id="bd77b-166">Preset15</span><span class="sxs-lookup"><span data-stu-id="bd77b-166">Preset15</span></span> | <span data-ttu-id="bd77b-167">Темно-красный</span><span class="sxs-lookup"><span data-stu-id="bd77b-167">DarkRed</span></span> |
| <span data-ttu-id="bd77b-168">Preset16</span><span class="sxs-lookup"><span data-stu-id="bd77b-168">Preset16</span></span> | <span data-ttu-id="bd77b-169">Темно-оранжевый</span><span class="sxs-lookup"><span data-stu-id="bd77b-169">DarkOrange</span></span> |
| <span data-ttu-id="bd77b-170">Preset17</span><span class="sxs-lookup"><span data-stu-id="bd77b-170">Preset17</span></span> | <span data-ttu-id="bd77b-171">Темно-коричневый</span><span class="sxs-lookup"><span data-stu-id="bd77b-171">DarkBrown</span></span> |
| <span data-ttu-id="bd77b-172">Preset18</span><span class="sxs-lookup"><span data-stu-id="bd77b-172">Preset18</span></span> | <span data-ttu-id="bd77b-173">Темно-желтый</span><span class="sxs-lookup"><span data-stu-id="bd77b-173">DarkYellow</span></span> |
| <span data-ttu-id="bd77b-174">Preset19</span><span class="sxs-lookup"><span data-stu-id="bd77b-174">Preset19</span></span> | <span data-ttu-id="bd77b-175">Темно-зеленый</span><span class="sxs-lookup"><span data-stu-id="bd77b-175">DarkGreen</span></span> |
| <span data-ttu-id="bd77b-176">Preset20</span><span class="sxs-lookup"><span data-stu-id="bd77b-176">Preset20</span></span> | <span data-ttu-id="bd77b-177">Темно-бирюзовый</span><span class="sxs-lookup"><span data-stu-id="bd77b-177">DarkTeal</span></span> |
| <span data-ttu-id="bd77b-178">Preset21</span><span class="sxs-lookup"><span data-stu-id="bd77b-178">Preset21</span></span> | <span data-ttu-id="bd77b-179">Темно-оливковый</span><span class="sxs-lookup"><span data-stu-id="bd77b-179">DarkOlive</span></span> |
| <span data-ttu-id="bd77b-180">Preset22</span><span class="sxs-lookup"><span data-stu-id="bd77b-180">Preset22</span></span> | <span data-ttu-id="bd77b-181">Темно-синий</span><span class="sxs-lookup"><span data-stu-id="bd77b-181">DarkBlue</span></span> |
| <span data-ttu-id="bd77b-182">Preset23</span><span class="sxs-lookup"><span data-stu-id="bd77b-182">Preset23</span></span> | <span data-ttu-id="bd77b-183">Темно-фиолетовый</span><span class="sxs-lookup"><span data-stu-id="bd77b-183">DarkPurple</span></span> |
| <span data-ttu-id="bd77b-184">Preset24</span><span class="sxs-lookup"><span data-stu-id="bd77b-184">Preset24</span></span> | <span data-ttu-id="bd77b-185">Темно-клюквенный</span><span class="sxs-lookup"><span data-stu-id="bd77b-185">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd77b-186">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bd77b-186">JSON representation</span></span>
<span data-ttu-id="bd77b-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd77b-187">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="bd77b-188">Методы</span><span class="sxs-lookup"><span data-stu-id="bd77b-188">Methods</span></span>
| <span data-ttu-id="bd77b-189">Метод</span><span class="sxs-lookup"><span data-stu-id="bd77b-189">Method</span></span>           | <span data-ttu-id="bd77b-190">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd77b-190">Return Type</span></span>    |<span data-ttu-id="bd77b-191">Описание</span><span class="sxs-lookup"><span data-stu-id="bd77b-191">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd77b-192">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="bd77b-192">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="bd77b-193">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bd77b-193">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="bd77b-194">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd77b-194">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="bd77b-195">Получение категории</span><span class="sxs-lookup"><span data-stu-id="bd77b-195">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="bd77b-196">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bd77b-196">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="bd77b-197">Получение свойств и отношений указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="bd77b-197">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="bd77b-198">Создание</span><span class="sxs-lookup"><span data-stu-id="bd77b-198">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="bd77b-199">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bd77b-199">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="bd77b-200">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd77b-200">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="bd77b-201">Обновление</span><span class="sxs-lookup"><span data-stu-id="bd77b-201">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="bd77b-202">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bd77b-202">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="bd77b-203">Обновление перезаписываемого свойства **color** указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="bd77b-203">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="bd77b-204">Delete</span><span class="sxs-lookup"><span data-stu-id="bd77b-204">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="bd77b-205">Нет</span><span class="sxs-lookup"><span data-stu-id="bd77b-205">None</span></span> |<span data-ttu-id="bd77b-206">Удаление указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="bd77b-206">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/outlookcategory.md:\r\n      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ]
}
-->
 


