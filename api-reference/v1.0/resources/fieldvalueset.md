---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: fieldValueSet
ms.openlocfilehash: b0e3accc05ddf10328f8d27f8798f865e579e529
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266606"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="3cc22-102">Ресурс fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="3cc22-102">FieldValueSet resource</span></span>

<span data-ttu-id="3cc22-103">Представляет значения столбца в ресурсе [listItem](listItem.md).</span><span class="sxs-lookup"><span data-stu-id="3cc22-103">Represents the column values in a [listItem](listItem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cc22-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3cc22-104">JSON representation</span></span>

<span data-ttu-id="3cc22-105">Ниже показано представление ресурса **fieldValueSet** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cc22-105">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
      "optionalProperties": ["Author", "AuthorLookupId", "Name", "Color", "Quantity" ],
       "baseType": "microsoft.graph.entity", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="3cc22-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cc22-106">Properties</span></span>

<span data-ttu-id="3cc22-107">Каждое отображаемое для пользователя поле в элементе **listItem** возвращается в виде пары имя-значение в объекте **fieldValueSet**.</span><span class="sxs-lookup"><span data-stu-id="3cc22-107">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="3cc22-108">В примере выше используется список, состоящий из четырех столбцов: **Author** (Автор), **Name** (Имя), **Color** (Цвет) и **Quantity** (Количество).</span><span class="sxs-lookup"><span data-stu-id="3cc22-108">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="3cc22-109">По умолчанию поля подстановки (например, поле `Author` выше) не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="3cc22-109">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="3cc22-110">Вместо этого сервер возвращает поле LookupId (например, поле `AuthorLookupId` выше), ссылающееся на элемент listItem, являющийся целевым элементом в подстановке.</span><span class="sxs-lookup"><span data-stu-id="3cc22-110">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="3cc22-111">Имя поля LookupId представляет собой исходное имя поля, за которым следует текст `LookupId`.</span><span class="sxs-lookup"><span data-stu-id="3cc22-111">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="3cc22-112">В одном запросе можно запросить до 12 полей подстановки.</span><span class="sxs-lookup"><span data-stu-id="3cc22-112">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="3cc22-113">Сервер возвратит значения подстановки, если запрос содержит оператор `select`, в котором указаны необходимые вам поля.</span><span class="sxs-lookup"><span data-stu-id="3cc22-113">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="3cc22-114">Пример.</span><span class="sxs-lookup"><span data-stu-id="3cc22-114">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="3cc22-115">В одном запросе вы можете запросить до 12 полей подстановки, а также любое количество "обычных" полей.</span><span class="sxs-lookup"><span data-stu-id="3cc22-115">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
