---
title: Тип ресурса outlookCategory
description: Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. В Outlook пользователь определяет категории в основном списке и может применять один или несколько пользовательских
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b480f676c39e64c87048765b4ccc145a077036d9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009253"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="c5459-104">Тип ресурса outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c5459-104">outlookCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5459-105">Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события.</span><span class="sxs-lookup"><span data-stu-id="c5459-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="c5459-106">В Outlook пользователь определяет категории в основном списке и может применить одну или несколько пользовательских категорий к элементу.</span><span class="sxs-lookup"><span data-stu-id="c5459-106">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="c5459-107">С помощью REST API вы можете [создавать](../api/outlookuser-post-mastercategories.md) и определять категории в основном списке категорий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5459-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="c5459-108">Вы также можете [получить этот основной список категорий](../api/outlookuser-list-mastercategories.md), [получить определенную категорию](../api/outlookcategory-get.md), [изменить](../api/outlookcategory-update.md) цвет, связанный с категорией, или [удалить](../api/outlookcategory-delete.md) категорию.</span><span class="sxs-lookup"><span data-stu-id="c5459-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="c5459-109">Вы можете применить категорию к списку, добавив значение свойства **displayName** категории в коллекцию **categories** элемента.</span><span class="sxs-lookup"><span data-stu-id="c5459-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="c5459-110">Ресурсы, которым могут быть назначены категории, включают [Контакты](contact.md), [события](event.md), [сообщения](message.md), [outlookTask](outlooktask.md)и [POST](post.md).</span><span class="sxs-lookup"><span data-stu-id="c5459-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="c5459-111">Каждой категории назначается 2 свойства: **displayName** и **color**.</span><span class="sxs-lookup"><span data-stu-id="c5459-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="c5459-112">Значение **displayName** должно быть уникальным в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5459-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="c5459-113">Однако значение свойства **color** может не быть уникальным. Несколько категорий в основном списке можно сопоставить с одним цветом.</span><span class="sxs-lookup"><span data-stu-id="c5459-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="c5459-114">Вы можете сопоставить до 25 различных цветов с категориями в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5459-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="c5459-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5459-115">Properties</span></span>
| <span data-ttu-id="c5459-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5459-116">Property</span></span>     | <span data-ttu-id="c5459-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c5459-117">Type</span></span>   |<span data-ttu-id="c5459-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c5459-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5459-119">displayName</span><span class="sxs-lookup"><span data-stu-id="c5459-119">displayName</span></span>|<span data-ttu-id="c5459-120">Строка</span><span class="sxs-lookup"><span data-stu-id="c5459-120">String</span></span>|<span data-ttu-id="c5459-121">Уникальное имя, обозначающее категорию в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5459-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="c5459-122">После создания категории изменить имя невозможно.</span><span class="sxs-lookup"><span data-stu-id="c5459-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="c5459-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5459-123">Read-only.</span></span>|
|<span data-ttu-id="c5459-124">color</span><span class="sxs-lookup"><span data-stu-id="c5459-124">color</span></span>|<span data-ttu-id="c5459-125">String</span><span class="sxs-lookup"><span data-stu-id="c5459-125">String</span></span>|<span data-ttu-id="c5459-126">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="c5459-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="c5459-127">См. примечание ниже.</span><span class="sxs-lookup"><span data-stu-id="c5459-127">See the note below.</span></span> |

> <span data-ttu-id="c5459-128">**Примечание**. Допустимые значения свойства **color** — предустановленные константы, например `None`, `preset0` и `preset1`.</span><span class="sxs-lookup"><span data-stu-id="c5459-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="c5459-129">Каждая предустановленная константа сопоставлена с цветом. Фактический цвет зависит от клиента Outlook, в котором отображаются категории.</span><span class="sxs-lookup"><span data-stu-id="c5459-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="c5459-130">В приведенной ниже таблице показаны цвета, сопоставленные с каждой предустановленной константой для классического клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="c5459-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="c5459-131">Предустановленная константа</span><span class="sxs-lookup"><span data-stu-id="c5459-131">Pre-set constant</span></span>  | <span data-ttu-id="c5459-132">Соответствующий цвет в Outlook</span><span class="sxs-lookup"><span data-stu-id="c5459-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5459-133">None</span><span class="sxs-lookup"><span data-stu-id="c5459-133">None</span></span> | <span data-ttu-id="c5459-134">Цвет не задан</span><span class="sxs-lookup"><span data-stu-id="c5459-134">No color mapped</span></span> |
| <span data-ttu-id="c5459-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="c5459-135">Preset0</span></span> | <span data-ttu-id="c5459-136">Красный</span><span class="sxs-lookup"><span data-stu-id="c5459-136">Red</span></span> |
| <span data-ttu-id="c5459-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="c5459-137">Preset1</span></span> | <span data-ttu-id="c5459-138">Оранжевый</span><span class="sxs-lookup"><span data-stu-id="c5459-138">Orange</span></span> |
| <span data-ttu-id="c5459-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="c5459-139">Preset2</span></span> | <span data-ttu-id="c5459-140">Коричневый</span><span class="sxs-lookup"><span data-stu-id="c5459-140">Brown</span></span> |
| <span data-ttu-id="c5459-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="c5459-141">Preset3</span></span> | <span data-ttu-id="c5459-142">Желтый</span><span class="sxs-lookup"><span data-stu-id="c5459-142">Yellow</span></span> |
| <span data-ttu-id="c5459-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="c5459-143">Preset4</span></span> | <span data-ttu-id="c5459-144">Зеленый</span><span class="sxs-lookup"><span data-stu-id="c5459-144">Green</span></span> |
| <span data-ttu-id="c5459-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="c5459-145">Preset5</span></span> | <span data-ttu-id="c5459-146">Сине-зеленый</span><span class="sxs-lookup"><span data-stu-id="c5459-146">Teal</span></span> |
| <span data-ttu-id="c5459-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="c5459-147">Preset6</span></span> | <span data-ttu-id="c5459-148">Оливковый</span><span class="sxs-lookup"><span data-stu-id="c5459-148">Olive</span></span> |
| <span data-ttu-id="c5459-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="c5459-149">Preset7</span></span> | <span data-ttu-id="c5459-150">Синий</span><span class="sxs-lookup"><span data-stu-id="c5459-150">Blue</span></span> |
| <span data-ttu-id="c5459-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="c5459-151">Preset8</span></span> | <span data-ttu-id="c5459-152">Сиреневый</span><span class="sxs-lookup"><span data-stu-id="c5459-152">Purple</span></span> |
| <span data-ttu-id="c5459-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="c5459-153">Preset9</span></span> | <span data-ttu-id="c5459-154">Клюквенный</span><span class="sxs-lookup"><span data-stu-id="c5459-154">Cranberry</span></span> |
| <span data-ttu-id="c5459-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="c5459-155">Preset10</span></span> | <span data-ttu-id="c5459-156">Стальной</span><span class="sxs-lookup"><span data-stu-id="c5459-156">Steel</span></span> |
| <span data-ttu-id="c5459-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="c5459-157">Preset11</span></span> | <span data-ttu-id="c5459-158">Темно-стальной</span><span class="sxs-lookup"><span data-stu-id="c5459-158">DarkSteel</span></span> |
| <span data-ttu-id="c5459-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="c5459-159">Preset12</span></span> | <span data-ttu-id="c5459-160">Серый</span><span class="sxs-lookup"><span data-stu-id="c5459-160">Gray</span></span> |
| <span data-ttu-id="c5459-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="c5459-161">Preset13</span></span> | <span data-ttu-id="c5459-162">Темно-серый</span><span class="sxs-lookup"><span data-stu-id="c5459-162">DarkGray</span></span> |
| <span data-ttu-id="c5459-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="c5459-163">Preset14</span></span> | <span data-ttu-id="c5459-164">Черный</span><span class="sxs-lookup"><span data-stu-id="c5459-164">Black</span></span> |
| <span data-ttu-id="c5459-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="c5459-165">Preset15</span></span> | <span data-ttu-id="c5459-166">Темно-красный</span><span class="sxs-lookup"><span data-stu-id="c5459-166">DarkRed</span></span> |
| <span data-ttu-id="c5459-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="c5459-167">Preset16</span></span> | <span data-ttu-id="c5459-168">Темно-оранжевый</span><span class="sxs-lookup"><span data-stu-id="c5459-168">DarkOrange</span></span> |
| <span data-ttu-id="c5459-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="c5459-169">Preset17</span></span> | <span data-ttu-id="c5459-170">Темно-коричневый</span><span class="sxs-lookup"><span data-stu-id="c5459-170">DarkBrown</span></span> |
| <span data-ttu-id="c5459-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="c5459-171">Preset18</span></span> | <span data-ttu-id="c5459-172">Темно-желтый</span><span class="sxs-lookup"><span data-stu-id="c5459-172">DarkYellow</span></span> |
| <span data-ttu-id="c5459-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="c5459-173">Preset19</span></span> | <span data-ttu-id="c5459-174">Темно-зеленый</span><span class="sxs-lookup"><span data-stu-id="c5459-174">DarkGreen</span></span> |
| <span data-ttu-id="c5459-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="c5459-175">Preset20</span></span> | <span data-ttu-id="c5459-176">Темно-бирюзовый</span><span class="sxs-lookup"><span data-stu-id="c5459-176">DarkTeal</span></span> |
| <span data-ttu-id="c5459-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="c5459-177">Preset21</span></span> | <span data-ttu-id="c5459-178">Темно-оливковый</span><span class="sxs-lookup"><span data-stu-id="c5459-178">DarkOlive</span></span> |
| <span data-ttu-id="c5459-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="c5459-179">Preset22</span></span> | <span data-ttu-id="c5459-180">Темно-синий</span><span class="sxs-lookup"><span data-stu-id="c5459-180">DarkBlue</span></span> |
| <span data-ttu-id="c5459-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="c5459-181">Preset23</span></span> | <span data-ttu-id="c5459-182">Темно-фиолетовый</span><span class="sxs-lookup"><span data-stu-id="c5459-182">DarkPurple</span></span> |
| <span data-ttu-id="c5459-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="c5459-183">Preset24</span></span> | <span data-ttu-id="c5459-184">Темно-клюквенный</span><span class="sxs-lookup"><span data-stu-id="c5459-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5459-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5459-185">JSON representation</span></span>
<span data-ttu-id="c5459-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5459-186">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="c5459-187">Методы</span><span class="sxs-lookup"><span data-stu-id="c5459-187">Methods</span></span>
| <span data-ttu-id="c5459-188">Метод</span><span class="sxs-lookup"><span data-stu-id="c5459-188">Method</span></span>           | <span data-ttu-id="c5459-189">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c5459-189">Return Type</span></span>    |<span data-ttu-id="c5459-190">Описание</span><span class="sxs-lookup"><span data-stu-id="c5459-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5459-191">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="c5459-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="c5459-192">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c5459-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="c5459-193">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5459-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="c5459-194">Получение категории</span><span class="sxs-lookup"><span data-stu-id="c5459-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="c5459-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c5459-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c5459-196">Получение свойств и отношений указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="c5459-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="c5459-197">Создание</span><span class="sxs-lookup"><span data-stu-id="c5459-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="c5459-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c5459-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c5459-199">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5459-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="c5459-200">Обновление</span><span class="sxs-lookup"><span data-stu-id="c5459-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="c5459-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c5459-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="c5459-202">Обновление перезаписываемого свойства **color** указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="c5459-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="c5459-203">Удаление</span><span class="sxs-lookup"><span data-stu-id="c5459-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="c5459-204">Нет</span><span class="sxs-lookup"><span data-stu-id="c5459-204">None</span></span> |<span data-ttu-id="c5459-205">Удаление указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="c5459-205">Delete the specified **outlookCategory** object.</span></span> |


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
 
