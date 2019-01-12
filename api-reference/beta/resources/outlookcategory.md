---
title: Тип ресурса outlookCategory
description: Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. В программе Outlook пользователь определяет категории в основной список и можно применить одно или несколько из следующих пользовательских
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9e4aa0c381e42522f80d933052ad7f0386643c60
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925170"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="8107e-104">Тип ресурса outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8107e-104">outlookCategory resource type</span></span>

> <span data-ttu-id="8107e-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8107e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8107e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8107e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8107e-107">Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события.</span><span class="sxs-lookup"><span data-stu-id="8107e-107">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="8107e-108">В программе Outlook пользователь определяет категории в основной список и можно применить один или несколько из следующих категорий пользовательских элементов.</span><span class="sxs-lookup"><span data-stu-id="8107e-108">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="8107e-109">С помощью REST API вы можете [создавать](../api/outlookuser-post-mastercategories.md) и определять категории в основном списке категорий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8107e-109">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="8107e-110">Вы также можете [получить этот основной список категорий](../api/outlookuser-list-mastercategories.md), [получить определенную категорию](../api/outlookcategory-get.md), [изменить](../api/outlookcategory-update.md) цвет, связанный с категорией, или [удалить](../api/outlookcategory-delete.md) категорию.</span><span class="sxs-lookup"><span data-stu-id="8107e-110">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="8107e-111">Вы можете применить категорию к списку, добавив значение свойства **displayName** категории в коллекцию **categories** элемента.</span><span class="sxs-lookup"><span data-stu-id="8107e-111">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="8107e-112">Ресурсы, которые можно назначить категории включают [контактов](contact.md), [событий](event.md), [сообщение](message.md), [outlookTask](outlooktask.md)и [публикации](post.md).</span><span class="sxs-lookup"><span data-stu-id="8107e-112">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="8107e-113">Каждой категории назначается 2 свойства: **displayName** и **color**.</span><span class="sxs-lookup"><span data-stu-id="8107e-113">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="8107e-114">Значение **displayName** должно быть уникальным в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="8107e-114">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="8107e-115">Однако значение свойства **color** может не быть уникальным. Несколько категорий в основном списке можно сопоставить с одним цветом.</span><span class="sxs-lookup"><span data-stu-id="8107e-115">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="8107e-116">Вы можете сопоставить до 25 различных цветов с категориями в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="8107e-116">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="8107e-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="8107e-117">Properties</span></span>
| <span data-ttu-id="8107e-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="8107e-118">Property</span></span>     | <span data-ttu-id="8107e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8107e-119">Type</span></span>   |<span data-ttu-id="8107e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8107e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8107e-121">displayName</span><span class="sxs-lookup"><span data-stu-id="8107e-121">displayName</span></span>|<span data-ttu-id="8107e-122">Строка</span><span class="sxs-lookup"><span data-stu-id="8107e-122">String</span></span>|<span data-ttu-id="8107e-123">Уникальное имя, обозначающее категорию в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8107e-123">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="8107e-124">После создания категории изменить имя невозможно.</span><span class="sxs-lookup"><span data-stu-id="8107e-124">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="8107e-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8107e-125">Read-only.</span></span>|
|<span data-ttu-id="8107e-126">color</span><span class="sxs-lookup"><span data-stu-id="8107e-126">color</span></span>|<span data-ttu-id="8107e-127">Строка</span><span class="sxs-lookup"><span data-stu-id="8107e-127">String</span></span>|<span data-ttu-id="8107e-128">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="8107e-128">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="8107e-129">См. примечание ниже.</span><span class="sxs-lookup"><span data-stu-id="8107e-129">See the note below.</span></span> |

> <span data-ttu-id="8107e-130">**Примечание**. Допустимые значения свойства **color** — предустановленные константы, например `None`, `preset0` и `preset1`.</span><span class="sxs-lookup"><span data-stu-id="8107e-130">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="8107e-131">Каждая предустановленная константа сопоставлена с цветом. Фактический цвет зависит от клиента Outlook, в котором отображаются категории.</span><span class="sxs-lookup"><span data-stu-id="8107e-131">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="8107e-132">В приведенной ниже таблице показаны цвета, сопоставленные с каждой предустановленной константой для классического клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="8107e-132">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="8107e-133">Предустановленная константа</span><span class="sxs-lookup"><span data-stu-id="8107e-133">Pre-set constant</span></span>  | <span data-ttu-id="8107e-134">Соответствующий цвет в Outlook</span><span class="sxs-lookup"><span data-stu-id="8107e-134">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8107e-135">None</span><span class="sxs-lookup"><span data-stu-id="8107e-135">None</span></span> | <span data-ttu-id="8107e-136">Цвет не задан</span><span class="sxs-lookup"><span data-stu-id="8107e-136">No color mapped</span></span> |
| <span data-ttu-id="8107e-137">Preset0</span><span class="sxs-lookup"><span data-stu-id="8107e-137">Preset0</span></span> | <span data-ttu-id="8107e-138">Красный</span><span class="sxs-lookup"><span data-stu-id="8107e-138">Red</span></span> |
| <span data-ttu-id="8107e-139">Preset1</span><span class="sxs-lookup"><span data-stu-id="8107e-139">Preset1</span></span> | <span data-ttu-id="8107e-140">Оранжевый</span><span class="sxs-lookup"><span data-stu-id="8107e-140">Orange</span></span> |
| <span data-ttu-id="8107e-141">Preset2</span><span class="sxs-lookup"><span data-stu-id="8107e-141">Preset2</span></span> | <span data-ttu-id="8107e-142">Коричневый</span><span class="sxs-lookup"><span data-stu-id="8107e-142">Brown</span></span> |
| <span data-ttu-id="8107e-143">Preset3</span><span class="sxs-lookup"><span data-stu-id="8107e-143">Preset3</span></span> | <span data-ttu-id="8107e-144">Желтый</span><span class="sxs-lookup"><span data-stu-id="8107e-144">Yellow</span></span> |
| <span data-ttu-id="8107e-145">Preset4</span><span class="sxs-lookup"><span data-stu-id="8107e-145">Preset4</span></span> | <span data-ttu-id="8107e-146">Зеленый</span><span class="sxs-lookup"><span data-stu-id="8107e-146">Green</span></span> |
| <span data-ttu-id="8107e-147">Preset5</span><span class="sxs-lookup"><span data-stu-id="8107e-147">Preset5</span></span> | <span data-ttu-id="8107e-148">Сине-зеленый</span><span class="sxs-lookup"><span data-stu-id="8107e-148">Teal</span></span> |
| <span data-ttu-id="8107e-149">Preset6</span><span class="sxs-lookup"><span data-stu-id="8107e-149">Preset6</span></span> | <span data-ttu-id="8107e-150">Оливковый</span><span class="sxs-lookup"><span data-stu-id="8107e-150">Olive</span></span> |
| <span data-ttu-id="8107e-151">Preset7</span><span class="sxs-lookup"><span data-stu-id="8107e-151">Preset7</span></span> | <span data-ttu-id="8107e-152">Синий</span><span class="sxs-lookup"><span data-stu-id="8107e-152">Blue</span></span> |
| <span data-ttu-id="8107e-153">Preset8</span><span class="sxs-lookup"><span data-stu-id="8107e-153">Preset8</span></span> | <span data-ttu-id="8107e-154">Сиреневый</span><span class="sxs-lookup"><span data-stu-id="8107e-154">Purple</span></span> |
| <span data-ttu-id="8107e-155">Preset9</span><span class="sxs-lookup"><span data-stu-id="8107e-155">Preset9</span></span> | <span data-ttu-id="8107e-156">Клюквенный</span><span class="sxs-lookup"><span data-stu-id="8107e-156">Cranberry</span></span> |
| <span data-ttu-id="8107e-157">Preset10</span><span class="sxs-lookup"><span data-stu-id="8107e-157">Preset10</span></span> | <span data-ttu-id="8107e-158">Стальной</span><span class="sxs-lookup"><span data-stu-id="8107e-158">Steel</span></span> |
| <span data-ttu-id="8107e-159">Preset11</span><span class="sxs-lookup"><span data-stu-id="8107e-159">Preset11</span></span> | <span data-ttu-id="8107e-160">Темно-стальной</span><span class="sxs-lookup"><span data-stu-id="8107e-160">DarkSteel</span></span> |
| <span data-ttu-id="8107e-161">Preset12</span><span class="sxs-lookup"><span data-stu-id="8107e-161">Preset12</span></span> | <span data-ttu-id="8107e-162">Серый</span><span class="sxs-lookup"><span data-stu-id="8107e-162">Gray</span></span> |
| <span data-ttu-id="8107e-163">Preset13</span><span class="sxs-lookup"><span data-stu-id="8107e-163">Preset13</span></span> | <span data-ttu-id="8107e-164">Темно-серый</span><span class="sxs-lookup"><span data-stu-id="8107e-164">DarkGray</span></span> |
| <span data-ttu-id="8107e-165">Preset14</span><span class="sxs-lookup"><span data-stu-id="8107e-165">Preset14</span></span> | <span data-ttu-id="8107e-166">Черный</span><span class="sxs-lookup"><span data-stu-id="8107e-166">Black</span></span> |
| <span data-ttu-id="8107e-167">Preset15</span><span class="sxs-lookup"><span data-stu-id="8107e-167">Preset15</span></span> | <span data-ttu-id="8107e-168">Темно-красный</span><span class="sxs-lookup"><span data-stu-id="8107e-168">DarkRed</span></span> |
| <span data-ttu-id="8107e-169">Preset16</span><span class="sxs-lookup"><span data-stu-id="8107e-169">Preset16</span></span> | <span data-ttu-id="8107e-170">Темно-оранжевый</span><span class="sxs-lookup"><span data-stu-id="8107e-170">DarkOrange</span></span> |
| <span data-ttu-id="8107e-171">Preset17</span><span class="sxs-lookup"><span data-stu-id="8107e-171">Preset17</span></span> | <span data-ttu-id="8107e-172">Темно-коричневый</span><span class="sxs-lookup"><span data-stu-id="8107e-172">DarkBrown</span></span> |
| <span data-ttu-id="8107e-173">Preset18</span><span class="sxs-lookup"><span data-stu-id="8107e-173">Preset18</span></span> | <span data-ttu-id="8107e-174">Темно-желтый</span><span class="sxs-lookup"><span data-stu-id="8107e-174">DarkYellow</span></span> |
| <span data-ttu-id="8107e-175">Preset19</span><span class="sxs-lookup"><span data-stu-id="8107e-175">Preset19</span></span> | <span data-ttu-id="8107e-176">Темно-зеленый</span><span class="sxs-lookup"><span data-stu-id="8107e-176">DarkGreen</span></span> |
| <span data-ttu-id="8107e-177">Preset20</span><span class="sxs-lookup"><span data-stu-id="8107e-177">Preset20</span></span> | <span data-ttu-id="8107e-178">Темно-бирюзовый</span><span class="sxs-lookup"><span data-stu-id="8107e-178">DarkTeal</span></span> |
| <span data-ttu-id="8107e-179">Preset21</span><span class="sxs-lookup"><span data-stu-id="8107e-179">Preset21</span></span> | <span data-ttu-id="8107e-180">Темно-оливковый</span><span class="sxs-lookup"><span data-stu-id="8107e-180">DarkOlive</span></span> |
| <span data-ttu-id="8107e-181">Preset22</span><span class="sxs-lookup"><span data-stu-id="8107e-181">Preset22</span></span> | <span data-ttu-id="8107e-182">Темно-синий</span><span class="sxs-lookup"><span data-stu-id="8107e-182">DarkBlue</span></span> |
| <span data-ttu-id="8107e-183">Preset23</span><span class="sxs-lookup"><span data-stu-id="8107e-183">Preset23</span></span> | <span data-ttu-id="8107e-184">Темно-фиолетовый</span><span class="sxs-lookup"><span data-stu-id="8107e-184">DarkPurple</span></span> |
| <span data-ttu-id="8107e-185">Preset24</span><span class="sxs-lookup"><span data-stu-id="8107e-185">Preset24</span></span> | <span data-ttu-id="8107e-186">Темно-клюквенный</span><span class="sxs-lookup"><span data-stu-id="8107e-186">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8107e-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8107e-187">JSON representation</span></span>
<span data-ttu-id="8107e-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8107e-188">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="8107e-189">Методы</span><span class="sxs-lookup"><span data-stu-id="8107e-189">Methods</span></span>
| <span data-ttu-id="8107e-190">Метод</span><span class="sxs-lookup"><span data-stu-id="8107e-190">Method</span></span>           | <span data-ttu-id="8107e-191">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8107e-191">Return Type</span></span>    |<span data-ttu-id="8107e-192">Описание</span><span class="sxs-lookup"><span data-stu-id="8107e-192">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8107e-193">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="8107e-193">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="8107e-194">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="8107e-194">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="8107e-195">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8107e-195">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="8107e-196">Получение категории</span><span class="sxs-lookup"><span data-stu-id="8107e-196">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="8107e-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8107e-197">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="8107e-198">Получение свойств и отношений указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="8107e-198">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="8107e-199">Создание</span><span class="sxs-lookup"><span data-stu-id="8107e-199">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="8107e-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8107e-200">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="8107e-201">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="8107e-201">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="8107e-202">Обновление</span><span class="sxs-lookup"><span data-stu-id="8107e-202">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="8107e-203">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="8107e-203">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="8107e-204">Обновление перезаписываемого свойства **color** указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="8107e-204">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="8107e-205">Удаление</span><span class="sxs-lookup"><span data-stu-id="8107e-205">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="8107e-206">Нет</span><span class="sxs-lookup"><span data-stu-id="8107e-206">None</span></span> |<span data-ttu-id="8107e-207">Удаление указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="8107e-207">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/beta/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 
