---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
ms.openlocfilehash: 63bbabccc540046961d31c91fe7b1fb9afaaf4f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027715"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="fea47-103">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="fea47-103">outlookUser resource type</span></span>


<span data-ttu-id="fea47-104">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="fea47-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="fea47-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fea47-105">Methods</span></span>

| <span data-ttu-id="fea47-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fea47-106">Method</span></span>           | <span data-ttu-id="fea47-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fea47-107">Return Type</span></span>    |<span data-ttu-id="fea47-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fea47-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fea47-109">Создание категории</span><span class="sxs-lookup"><span data-stu-id="fea47-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="fea47-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="fea47-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="fea47-111">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="fea47-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="fea47-112">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="fea47-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="fea47-113">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="fea47-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="fea47-114">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fea47-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="fea47-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="fea47-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="fea47-116">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="fea47-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="fea47-117">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="fea47-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="fea47-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="fea47-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="fea47-119">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="fea47-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="fea47-120">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="fea47-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="fea47-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="fea47-121">Properties</span></span>
<span data-ttu-id="fea47-122">Нет</span><span class="sxs-lookup"><span data-stu-id="fea47-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fea47-123">Связи</span><span class="sxs-lookup"><span data-stu-id="fea47-123">Relationships</span></span>
| <span data-ttu-id="fea47-124">Связь</span><span class="sxs-lookup"><span data-stu-id="fea47-124">Relationship</span></span> | <span data-ttu-id="fea47-125">Тип</span><span class="sxs-lookup"><span data-stu-id="fea47-125">Type</span></span>   |<span data-ttu-id="fea47-126">Описание</span><span class="sxs-lookup"><span data-stu-id="fea47-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fea47-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="fea47-127">masterCategories</span></span>|<span data-ttu-id="fea47-128">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="fea47-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="fea47-129">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fea47-129">A list of categories defined for the user.</span></span> | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->