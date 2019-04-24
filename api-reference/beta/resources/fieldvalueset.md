---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: ed10b586ee55ccd32e81b03bdc6359ee13605877
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506526"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="4995e-102">Ресурс fieldValueSet</span><span class="sxs-lookup"><span data-stu-id="4995e-102">FieldValueSet resource</span></span>

<span data-ttu-id="4995e-103">Представляет значения столбца в ресурсе [listItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="4995e-103">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4995e-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4995e-104">JSON representation</span></span>

<span data-ttu-id="4995e-105">Ниже показано представление ресурса **fieldValueSet** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4995e-105">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="4995e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4995e-106">Properties</span></span>

<span data-ttu-id="4995e-107">Каждое отображаемое для пользователя поле в элементе **listItem** возвращается в виде пары имя-значение в объекте **fieldValueSet**.</span><span class="sxs-lookup"><span data-stu-id="4995e-107">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="4995e-108">В примере выше используется список, состоящий из четырех столбцов: **Author** (Автор), **Name** (Имя), **Color** (Цвет) и **Quantity** (Количество).</span><span class="sxs-lookup"><span data-stu-id="4995e-108">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="4995e-109">По умолчанию поля подстановки (например, поле `Author` выше) не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="4995e-109">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="4995e-110">Вместо этого сервер возвращает поле LookupId (например, поле `AuthorLookupId` выше), ссылающееся на элемент listItem, являющийся целевым элементом в подстановке.</span><span class="sxs-lookup"><span data-stu-id="4995e-110">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="4995e-111">Имя поля LookupId представляет собой исходное имя поля, за которым следует текст `LookupId`.</span><span class="sxs-lookup"><span data-stu-id="4995e-111">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="4995e-112">В одном запросе можно запросить до 12 полей подстановки.</span><span class="sxs-lookup"><span data-stu-id="4995e-112">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="4995e-113">Сервер возвратит значения подстановки, если запрос содержит оператор `select`, в котором указаны необходимые вам поля.</span><span class="sxs-lookup"><span data-stu-id="4995e-113">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="4995e-114">Пример.</span><span class="sxs-lookup"><span data-stu-id="4995e-114">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="4995e-115">В одном запросе вы можете запросить до 12 полей подстановки, а также любое количество "обычных" полей.</span><span class="sxs-lookup"><span data-stu-id="4995e-115">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
