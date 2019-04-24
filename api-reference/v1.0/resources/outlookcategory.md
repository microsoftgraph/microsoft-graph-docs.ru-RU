---
title: Тип ресурса outlookCategory
description: Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. Пользователь определяет категории в основном списке и может применять один или несколько пользовательских
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 490ecaf2e6303cc943646dbed99b3202b8d57525
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462654"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="a7145-104">Тип ресурса outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a7145-104">outlookCategory resource type</span></span>


<span data-ttu-id="a7145-105">Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события.</span><span class="sxs-lookup"><span data-stu-id="a7145-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="a7145-106">Пользователь определяет категории в основном списке и может применить одну или несколько из них к элементу.</span><span class="sxs-lookup"><span data-stu-id="a7145-106">The user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="a7145-107">С помощью REST API вы можете [создавать](../api/outlookuser-post-mastercategories.md) и определять категории в основном списке категорий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7145-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="a7145-108">Вы также можете [получить этот основной список категорий](../api/outlookuser-list-mastercategories.md), [получить определенную категорию](../api/outlookcategory-get.md), [изменить](../api/outlookcategory-update.md) цвет, связанный с категорией, или [удалить](../api/outlookcategory-delete.md) категорию.</span><span class="sxs-lookup"><span data-stu-id="a7145-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="a7145-109">Вы можете применить категорию к списку, добавив значение свойства **displayName** категории в коллекцию **categories** элемента.</span><span class="sxs-lookup"><span data-stu-id="a7145-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="a7145-110">К ресурсам, которым можно назначать категории, относятся [contact](contact.md), [event](event.md), [message](message.md) и [post](post.md).</span><span class="sxs-lookup"><span data-stu-id="a7145-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), and [post](post.md).</span></span>   

<span data-ttu-id="a7145-111">Каждой категории назначается 2 свойства: **displayName** и **color**.</span><span class="sxs-lookup"><span data-stu-id="a7145-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="a7145-112">Значение **displayName** должно быть уникальным в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7145-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="a7145-113">Однако значение свойства **color** может не быть уникальным. Несколько категорий в основном списке можно сопоставить с одним цветом.</span><span class="sxs-lookup"><span data-stu-id="a7145-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="a7145-114">Вы можете сопоставить до 25 различных цветов с категориями в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7145-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="a7145-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7145-115">Properties</span></span>
| <span data-ttu-id="a7145-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7145-116">Property</span></span>     | <span data-ttu-id="a7145-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a7145-117">Type</span></span>   |<span data-ttu-id="a7145-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a7145-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7145-119">displayName</span><span class="sxs-lookup"><span data-stu-id="a7145-119">displayName</span></span>|<span data-ttu-id="a7145-120">String</span><span class="sxs-lookup"><span data-stu-id="a7145-120">String</span></span>|<span data-ttu-id="a7145-121">Уникальное имя, обозначающее категорию в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7145-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="a7145-122">После создания категории изменить имя невозможно.</span><span class="sxs-lookup"><span data-stu-id="a7145-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="a7145-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7145-123">Read-only.</span></span>|
|<span data-ttu-id="a7145-124">color</span><span class="sxs-lookup"><span data-stu-id="a7145-124">color</span></span>|<span data-ttu-id="a7145-125">Категориколор</span><span class="sxs-lookup"><span data-stu-id="a7145-125">categoryColor</span></span>|<span data-ttu-id="a7145-126">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="a7145-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="a7145-127">См. примечание ниже.</span><span class="sxs-lookup"><span data-stu-id="a7145-127">See the note below.</span></span> |

> <span data-ttu-id="a7145-128">**Примечание**. Допустимые значения свойства **color** — предустановленные константы, например `None`, `preset0` и `preset1`.</span><span class="sxs-lookup"><span data-stu-id="a7145-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="a7145-129">Каждая предустановленная константа сопоставлена с цветом. Фактический цвет зависит от клиента Outlook, в котором отображаются категории.</span><span class="sxs-lookup"><span data-stu-id="a7145-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="a7145-130">В приведенной ниже таблице показаны цвета, сопоставленные с каждой предустановленной константой для классического клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="a7145-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 

| <span data-ttu-id="a7145-131">Предустановленная константа</span><span class="sxs-lookup"><span data-stu-id="a7145-131">Pre-set constant</span></span>  | <span data-ttu-id="a7145-132">Соответствующий цвет в Outlook</span><span class="sxs-lookup"><span data-stu-id="a7145-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7145-133">None</span><span class="sxs-lookup"><span data-stu-id="a7145-133">None</span></span> | <span data-ttu-id="a7145-134">Цвет не задан</span><span class="sxs-lookup"><span data-stu-id="a7145-134">No color mapped</span></span> |
| <span data-ttu-id="a7145-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="a7145-135">Preset0</span></span> | <span data-ttu-id="a7145-136">Красный</span><span class="sxs-lookup"><span data-stu-id="a7145-136">Red</span></span> |
| <span data-ttu-id="a7145-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="a7145-137">Preset1</span></span> | <span data-ttu-id="a7145-138">Оранжевый</span><span class="sxs-lookup"><span data-stu-id="a7145-138">Orange</span></span> |
| <span data-ttu-id="a7145-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="a7145-139">Preset2</span></span> | <span data-ttu-id="a7145-140">Коричневый</span><span class="sxs-lookup"><span data-stu-id="a7145-140">Brown</span></span> |
| <span data-ttu-id="a7145-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="a7145-141">Preset3</span></span> | <span data-ttu-id="a7145-142">Желтый</span><span class="sxs-lookup"><span data-stu-id="a7145-142">Yellow</span></span> |
| <span data-ttu-id="a7145-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="a7145-143">Preset4</span></span> | <span data-ttu-id="a7145-144">Зеленый</span><span class="sxs-lookup"><span data-stu-id="a7145-144">Green</span></span> |
| <span data-ttu-id="a7145-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="a7145-145">Preset5</span></span> | <span data-ttu-id="a7145-146">Сине-зеленый</span><span class="sxs-lookup"><span data-stu-id="a7145-146">Teal</span></span> |
| <span data-ttu-id="a7145-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="a7145-147">Preset6</span></span> | <span data-ttu-id="a7145-148">Оливковый</span><span class="sxs-lookup"><span data-stu-id="a7145-148">Olive</span></span> |
| <span data-ttu-id="a7145-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="a7145-149">Preset7</span></span> | <span data-ttu-id="a7145-150">Синий</span><span class="sxs-lookup"><span data-stu-id="a7145-150">Blue</span></span> |
| <span data-ttu-id="a7145-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="a7145-151">Preset8</span></span> | <span data-ttu-id="a7145-152">Сиреневый</span><span class="sxs-lookup"><span data-stu-id="a7145-152">Purple</span></span> |
| <span data-ttu-id="a7145-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="a7145-153">Preset9</span></span> | <span data-ttu-id="a7145-154">Клюквенный</span><span class="sxs-lookup"><span data-stu-id="a7145-154">Cranberry</span></span> |
| <span data-ttu-id="a7145-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="a7145-155">Preset10</span></span> | <span data-ttu-id="a7145-156">Стальной</span><span class="sxs-lookup"><span data-stu-id="a7145-156">Steel</span></span> |
| <span data-ttu-id="a7145-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="a7145-157">Preset11</span></span> | <span data-ttu-id="a7145-158">Темно-стальной</span><span class="sxs-lookup"><span data-stu-id="a7145-158">DarkSteel</span></span> |
| <span data-ttu-id="a7145-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="a7145-159">Preset12</span></span> | <span data-ttu-id="a7145-160">Серый</span><span class="sxs-lookup"><span data-stu-id="a7145-160">Gray</span></span> |
| <span data-ttu-id="a7145-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="a7145-161">Preset13</span></span> | <span data-ttu-id="a7145-162">Темно-серый</span><span class="sxs-lookup"><span data-stu-id="a7145-162">DarkGray</span></span> |
| <span data-ttu-id="a7145-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="a7145-163">Preset14</span></span> | <span data-ttu-id="a7145-164">Черный</span><span class="sxs-lookup"><span data-stu-id="a7145-164">Black</span></span> |
| <span data-ttu-id="a7145-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="a7145-165">Preset15</span></span> | <span data-ttu-id="a7145-166">Темно-красный</span><span class="sxs-lookup"><span data-stu-id="a7145-166">DarkRed</span></span> |
| <span data-ttu-id="a7145-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="a7145-167">Preset16</span></span> | <span data-ttu-id="a7145-168">Темно-оранжевый</span><span class="sxs-lookup"><span data-stu-id="a7145-168">DarkOrange</span></span> |
| <span data-ttu-id="a7145-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="a7145-169">Preset17</span></span> | <span data-ttu-id="a7145-170">Темно-коричневый</span><span class="sxs-lookup"><span data-stu-id="a7145-170">DarkBrown</span></span> |
| <span data-ttu-id="a7145-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="a7145-171">Preset18</span></span> | <span data-ttu-id="a7145-172">Темно-желтый</span><span class="sxs-lookup"><span data-stu-id="a7145-172">DarkYellow</span></span> |
| <span data-ttu-id="a7145-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="a7145-173">Preset19</span></span> | <span data-ttu-id="a7145-174">Темно-зеленый</span><span class="sxs-lookup"><span data-stu-id="a7145-174">DarkGreen</span></span> |
| <span data-ttu-id="a7145-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="a7145-175">Preset20</span></span> | <span data-ttu-id="a7145-176">Темно-бирюзовый</span><span class="sxs-lookup"><span data-stu-id="a7145-176">DarkTeal</span></span> |
| <span data-ttu-id="a7145-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="a7145-177">Preset21</span></span> | <span data-ttu-id="a7145-178">Темно-оливковый</span><span class="sxs-lookup"><span data-stu-id="a7145-178">DarkOlive</span></span> |
| <span data-ttu-id="a7145-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="a7145-179">Preset22</span></span> | <span data-ttu-id="a7145-180">Темно-синий</span><span class="sxs-lookup"><span data-stu-id="a7145-180">DarkBlue</span></span> |
| <span data-ttu-id="a7145-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="a7145-181">Preset23</span></span> | <span data-ttu-id="a7145-182">Темно-фиолетовый</span><span class="sxs-lookup"><span data-stu-id="a7145-182">DarkPurple</span></span> |
| <span data-ttu-id="a7145-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="a7145-183">Preset24</span></span> | <span data-ttu-id="a7145-184">Темно-клюквенный</span><span class="sxs-lookup"><span data-stu-id="a7145-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a7145-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7145-185">JSON representation</span></span>
<span data-ttu-id="a7145-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7145-186">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="a7145-187">Методы</span><span class="sxs-lookup"><span data-stu-id="a7145-187">Methods</span></span>
| <span data-ttu-id="a7145-188">Метод</span><span class="sxs-lookup"><span data-stu-id="a7145-188">Method</span></span>           | <span data-ttu-id="a7145-189">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a7145-189">Return Type</span></span>    |<span data-ttu-id="a7145-190">Описание</span><span class="sxs-lookup"><span data-stu-id="a7145-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a7145-191">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="a7145-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="a7145-192">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="a7145-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="a7145-193">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7145-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="a7145-194">Получение категории</span><span class="sxs-lookup"><span data-stu-id="a7145-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="a7145-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a7145-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="a7145-196">Получение свойств и отношений указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="a7145-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="a7145-197">Создание</span><span class="sxs-lookup"><span data-stu-id="a7145-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="a7145-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a7145-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="a7145-199">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7145-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="a7145-200">Обновление</span><span class="sxs-lookup"><span data-stu-id="a7145-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="a7145-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a7145-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="a7145-202">Обновление перезаписываемого свойства **color** указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="a7145-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="a7145-203">Удаление</span><span class="sxs-lookup"><span data-stu-id="a7145-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="a7145-204">Нет</span><span class="sxs-lookup"><span data-stu-id="a7145-204">None</span></span> |<span data-ttu-id="a7145-205">Удаление указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="a7145-205">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 
