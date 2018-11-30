---
title: Тип ресурса outlookCategory
description: Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. В программе Outlook пользователь определяет категории в основной список и можно применить одно или несколько из следующих пользовательских
ms.openlocfilehash: 073441894989ee4193018a404b0472a5f1562e4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075560"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="37759-104">Тип ресурса outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37759-104">outlookCategory resource type</span></span>

> <span data-ttu-id="37759-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37759-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37759-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37759-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37759-107">Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события.</span><span class="sxs-lookup"><span data-stu-id="37759-107">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="37759-108">В программе Outlook пользователь определяет категории в основной список и можно применить один или несколько из следующих категорий пользовательских элементов.</span><span class="sxs-lookup"><span data-stu-id="37759-108">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="37759-109">С помощью REST API вы можете [создавать](../api/outlookuser-post-mastercategories.md) и определять категории в основном списке категорий для пользователя.</span><span class="sxs-lookup"><span data-stu-id="37759-109">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="37759-110">Вы также можете [получить этот основной список категорий](../api/outlookuser-list-mastercategories.md), [получить определенную категорию](../api/outlookcategory-get.md), [изменить](../api/outlookcategory-update.md) цвет, связанный с категорией, или [удалить](../api/outlookcategory-delete.md) категорию.</span><span class="sxs-lookup"><span data-stu-id="37759-110">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="37759-111">Вы можете применить категорию к списку, добавив значение свойства **displayName** категории в коллекцию **categories** элемента.</span><span class="sxs-lookup"><span data-stu-id="37759-111">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="37759-112">Ресурсы, которые можно назначить категории включают [контактов](contact.md), [событий](event.md), [сообщение](message.md), [outlookTask](outlooktask.md)и [публикации](post.md).</span><span class="sxs-lookup"><span data-stu-id="37759-112">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="37759-113">Каждой категории назначается 2 свойства: **displayName** и **color**.</span><span class="sxs-lookup"><span data-stu-id="37759-113">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="37759-114">Значение **displayName** должно быть уникальным в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="37759-114">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="37759-115">Однако значение свойства **color** может не быть уникальным. Несколько категорий в основном списке можно сопоставить с одним цветом.</span><span class="sxs-lookup"><span data-stu-id="37759-115">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="37759-116">Вы можете сопоставить до 25 различных цветов с категориями в основном списке пользователя.</span><span class="sxs-lookup"><span data-stu-id="37759-116">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="37759-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="37759-117">Properties</span></span>
| <span data-ttu-id="37759-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="37759-118">Property</span></span>     | <span data-ttu-id="37759-119">Тип</span><span class="sxs-lookup"><span data-stu-id="37759-119">Type</span></span>   |<span data-ttu-id="37759-120">Описание</span><span class="sxs-lookup"><span data-stu-id="37759-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37759-121">displayName</span><span class="sxs-lookup"><span data-stu-id="37759-121">displayName</span></span>|<span data-ttu-id="37759-122">Строка</span><span class="sxs-lookup"><span data-stu-id="37759-122">String</span></span>|<span data-ttu-id="37759-123">Уникальное имя, обозначающее категорию в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="37759-123">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="37759-124">После создания категории изменить имя невозможно.</span><span class="sxs-lookup"><span data-stu-id="37759-124">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="37759-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37759-125">Read-only.</span></span>|
|<span data-ttu-id="37759-126">color</span><span class="sxs-lookup"><span data-stu-id="37759-126">color</span></span>|<span data-ttu-id="37759-127">String</span><span class="sxs-lookup"><span data-stu-id="37759-127">String</span></span>|<span data-ttu-id="37759-128">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="37759-128">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="37759-129">См. примечание ниже.</span><span class="sxs-lookup"><span data-stu-id="37759-129">See the note below.</span></span> |

> <span data-ttu-id="37759-130">**Примечание**. Допустимые значения свойства **color** — предустановленные константы, например `None`, `preset0` и `preset1`.</span><span class="sxs-lookup"><span data-stu-id="37759-130">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="37759-131">Каждая предустановленная константа сопоставлена с цветом. Фактический цвет зависит от клиента Outlook, в котором отображаются категории.</span><span class="sxs-lookup"><span data-stu-id="37759-131">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="37759-132">В приведенной ниже таблице показаны цвета, сопоставленные с каждой предустановленной константой для классического клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="37759-132">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="37759-133">Предустановленная константа</span><span class="sxs-lookup"><span data-stu-id="37759-133">Pre-set constant</span></span>  | <span data-ttu-id="37759-134">Соответствующий цвет в Outlook</span><span class="sxs-lookup"><span data-stu-id="37759-134">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="37759-135">None</span><span class="sxs-lookup"><span data-stu-id="37759-135">None</span></span> | <span data-ttu-id="37759-136">Цвет не задан</span><span class="sxs-lookup"><span data-stu-id="37759-136">No color mapped</span></span> |
| <span data-ttu-id="37759-137">Preset0</span><span class="sxs-lookup"><span data-stu-id="37759-137">Preset0</span></span> | <span data-ttu-id="37759-138">Красный</span><span class="sxs-lookup"><span data-stu-id="37759-138">Red</span></span> |
| <span data-ttu-id="37759-139">Preset1</span><span class="sxs-lookup"><span data-stu-id="37759-139">Preset1</span></span> | <span data-ttu-id="37759-140">Оранжевый</span><span class="sxs-lookup"><span data-stu-id="37759-140">Orange</span></span> |
| <span data-ttu-id="37759-141">Preset2</span><span class="sxs-lookup"><span data-stu-id="37759-141">Preset2</span></span> | <span data-ttu-id="37759-142">Коричневый</span><span class="sxs-lookup"><span data-stu-id="37759-142">Brown</span></span> |
| <span data-ttu-id="37759-143">Preset3</span><span class="sxs-lookup"><span data-stu-id="37759-143">Preset3</span></span> | <span data-ttu-id="37759-144">Желтый</span><span class="sxs-lookup"><span data-stu-id="37759-144">Yellow</span></span> |
| <span data-ttu-id="37759-145">Preset4</span><span class="sxs-lookup"><span data-stu-id="37759-145">Preset4</span></span> | <span data-ttu-id="37759-146">Зеленый</span><span class="sxs-lookup"><span data-stu-id="37759-146">Green</span></span> |
| <span data-ttu-id="37759-147">Preset5</span><span class="sxs-lookup"><span data-stu-id="37759-147">Preset5</span></span> | <span data-ttu-id="37759-148">Сине-зеленый</span><span class="sxs-lookup"><span data-stu-id="37759-148">Teal</span></span> |
| <span data-ttu-id="37759-149">Preset6</span><span class="sxs-lookup"><span data-stu-id="37759-149">Preset6</span></span> | <span data-ttu-id="37759-150">Оливковый</span><span class="sxs-lookup"><span data-stu-id="37759-150">Olive</span></span> |
| <span data-ttu-id="37759-151">Preset7</span><span class="sxs-lookup"><span data-stu-id="37759-151">Preset7</span></span> | <span data-ttu-id="37759-152">Синий</span><span class="sxs-lookup"><span data-stu-id="37759-152">Blue</span></span> |
| <span data-ttu-id="37759-153">Preset8</span><span class="sxs-lookup"><span data-stu-id="37759-153">Preset8</span></span> | <span data-ttu-id="37759-154">Сиреневый</span><span class="sxs-lookup"><span data-stu-id="37759-154">Purple</span></span> |
| <span data-ttu-id="37759-155">Preset9</span><span class="sxs-lookup"><span data-stu-id="37759-155">Preset9</span></span> | <span data-ttu-id="37759-156">Клюквенный</span><span class="sxs-lookup"><span data-stu-id="37759-156">Cranberry</span></span> |
| <span data-ttu-id="37759-157">Preset10</span><span class="sxs-lookup"><span data-stu-id="37759-157">Preset10</span></span> | <span data-ttu-id="37759-158">Стальной</span><span class="sxs-lookup"><span data-stu-id="37759-158">Steel</span></span> |
| <span data-ttu-id="37759-159">Preset11</span><span class="sxs-lookup"><span data-stu-id="37759-159">Preset11</span></span> | <span data-ttu-id="37759-160">Темно-стальной</span><span class="sxs-lookup"><span data-stu-id="37759-160">DarkSteel</span></span> |
| <span data-ttu-id="37759-161">Preset12</span><span class="sxs-lookup"><span data-stu-id="37759-161">Preset12</span></span> | <span data-ttu-id="37759-162">Серый</span><span class="sxs-lookup"><span data-stu-id="37759-162">Gray</span></span> |
| <span data-ttu-id="37759-163">Preset13</span><span class="sxs-lookup"><span data-stu-id="37759-163">Preset13</span></span> | <span data-ttu-id="37759-164">Темно-серый</span><span class="sxs-lookup"><span data-stu-id="37759-164">DarkGray</span></span> |
| <span data-ttu-id="37759-165">Preset14</span><span class="sxs-lookup"><span data-stu-id="37759-165">Preset14</span></span> | <span data-ttu-id="37759-166">Черный</span><span class="sxs-lookup"><span data-stu-id="37759-166">Black</span></span> |
| <span data-ttu-id="37759-167">Preset15</span><span class="sxs-lookup"><span data-stu-id="37759-167">Preset15</span></span> | <span data-ttu-id="37759-168">Темно-красный</span><span class="sxs-lookup"><span data-stu-id="37759-168">DarkRed</span></span> |
| <span data-ttu-id="37759-169">Preset16</span><span class="sxs-lookup"><span data-stu-id="37759-169">Preset16</span></span> | <span data-ttu-id="37759-170">Темно-оранжевый</span><span class="sxs-lookup"><span data-stu-id="37759-170">DarkOrange</span></span> |
| <span data-ttu-id="37759-171">Preset17</span><span class="sxs-lookup"><span data-stu-id="37759-171">Preset17</span></span> | <span data-ttu-id="37759-172">Темно-коричневый</span><span class="sxs-lookup"><span data-stu-id="37759-172">DarkBrown</span></span> |
| <span data-ttu-id="37759-173">Preset18</span><span class="sxs-lookup"><span data-stu-id="37759-173">Preset18</span></span> | <span data-ttu-id="37759-174">Темно-желтый</span><span class="sxs-lookup"><span data-stu-id="37759-174">DarkYellow</span></span> |
| <span data-ttu-id="37759-175">Preset19</span><span class="sxs-lookup"><span data-stu-id="37759-175">Preset19</span></span> | <span data-ttu-id="37759-176">Темно-зеленый</span><span class="sxs-lookup"><span data-stu-id="37759-176">DarkGreen</span></span> |
| <span data-ttu-id="37759-177">Preset20</span><span class="sxs-lookup"><span data-stu-id="37759-177">Preset20</span></span> | <span data-ttu-id="37759-178">Темно-бирюзовый</span><span class="sxs-lookup"><span data-stu-id="37759-178">DarkTeal</span></span> |
| <span data-ttu-id="37759-179">Preset21</span><span class="sxs-lookup"><span data-stu-id="37759-179">Preset21</span></span> | <span data-ttu-id="37759-180">Темно-оливковый</span><span class="sxs-lookup"><span data-stu-id="37759-180">DarkOlive</span></span> |
| <span data-ttu-id="37759-181">Preset22</span><span class="sxs-lookup"><span data-stu-id="37759-181">Preset22</span></span> | <span data-ttu-id="37759-182">Темно-синий</span><span class="sxs-lookup"><span data-stu-id="37759-182">DarkBlue</span></span> |
| <span data-ttu-id="37759-183">Preset23</span><span class="sxs-lookup"><span data-stu-id="37759-183">Preset23</span></span> | <span data-ttu-id="37759-184">Темно-фиолетовый</span><span class="sxs-lookup"><span data-stu-id="37759-184">DarkPurple</span></span> |
| <span data-ttu-id="37759-185">Preset24</span><span class="sxs-lookup"><span data-stu-id="37759-185">Preset24</span></span> | <span data-ttu-id="37759-186">Темно-клюквенный</span><span class="sxs-lookup"><span data-stu-id="37759-186">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37759-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37759-187">JSON representation</span></span>
<span data-ttu-id="37759-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37759-188">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="37759-189">Методы</span><span class="sxs-lookup"><span data-stu-id="37759-189">Methods</span></span>
| <span data-ttu-id="37759-190">Метод</span><span class="sxs-lookup"><span data-stu-id="37759-190">Method</span></span>           | <span data-ttu-id="37759-191">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="37759-191">Return Type</span></span>    |<span data-ttu-id="37759-192">Описание</span><span class="sxs-lookup"><span data-stu-id="37759-192">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37759-193">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="37759-193">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="37759-194">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="37759-194">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="37759-195">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="37759-195">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="37759-196">Получение категории</span><span class="sxs-lookup"><span data-stu-id="37759-196">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="37759-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37759-197">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="37759-198">Получение свойств и отношений указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="37759-198">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="37759-199">Создание</span><span class="sxs-lookup"><span data-stu-id="37759-199">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="37759-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37759-200">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="37759-201">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="37759-201">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="37759-202">Обновление</span><span class="sxs-lookup"><span data-stu-id="37759-202">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="37759-203">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37759-203">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="37759-204">Обновление перезаписываемого свойства **color** указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="37759-204">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="37759-205">Удаление</span><span class="sxs-lookup"><span data-stu-id="37759-205">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="37759-206">Нет</span><span class="sxs-lookup"><span data-stu-id="37759-206">None</span></span> |<span data-ttu-id="37759-207">Удаление указанного объекта **outlookCategory**.</span><span class="sxs-lookup"><span data-stu-id="37759-207">Delete the specified **outlookCategory** object.</span></span> |


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
 