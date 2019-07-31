---
author: JeremyKelley
description: Представляет значения столбца в ресурсе listItem.
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: dab7c315174342f68c6fcb045e46d7da9d32f06a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972049"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="82180-103">Ресурс fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="82180-103">FieldValueSet resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82180-104">Представляет значения столбца в ресурсе [listItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="82180-104">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82180-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="82180-105">JSON representation</span></span>

<span data-ttu-id="82180-106">Ниже показано представление ресурса **fieldValueSet** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82180-106">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="82180-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="82180-107">Properties</span></span>

<span data-ttu-id="82180-108">Каждое отображаемое для пользователя поле в элементе **listItem** возвращается в виде пары имя-значение в объекте **fieldValueSet**.</span><span class="sxs-lookup"><span data-stu-id="82180-108">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="82180-109">В примере выше используется список, состоящий из четырех столбцов: **Author** (Автор), **Name** (Имя), **Color** (Цвет) и **Quantity** (Количество).</span><span class="sxs-lookup"><span data-stu-id="82180-109">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="82180-110">По умолчанию поля подстановки (например, поле `Author` выше) не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="82180-110">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="82180-111">Вместо этого сервер возвращает поле LookupId (например, поле `AuthorLookupId` выше), ссылающееся на элемент listItem, являющийся целевым элементом в подстановке.</span><span class="sxs-lookup"><span data-stu-id="82180-111">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="82180-112">Имя поля LookupId представляет собой исходное имя поля, за которым следует текст `LookupId`.</span><span class="sxs-lookup"><span data-stu-id="82180-112">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="82180-113">В одном запросе можно запросить до 12 полей подстановки.</span><span class="sxs-lookup"><span data-stu-id="82180-113">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="82180-114">Сервер возвратит значения подстановки, если запрос содержит оператор `select`, в котором указаны необходимые вам поля.</span><span class="sxs-lookup"><span data-stu-id="82180-114">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="82180-115">Пример.</span><span class="sxs-lookup"><span data-stu-id="82180-115">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="82180-116">В одном запросе вы можете запросить до 12 полей подстановки, а также любое количество "обычных" полей.</span><span class="sxs-lookup"><span data-stu-id="82180-116">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet",
  "suppressions": []
}
-->
