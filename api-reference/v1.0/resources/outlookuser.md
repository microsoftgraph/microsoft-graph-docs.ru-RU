---
title: Тип ресурса outlookUser
description: Представляет службы Outlook, доступные пользователю.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 32014d4d9591cb72adf16434ee99d4d57255bfb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066266"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="bf2b7-103">Тип ресурса outlookUser</span><span class="sxs-lookup"><span data-stu-id="bf2b7-103">outlookUser resource type</span></span>

<span data-ttu-id="bf2b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf2b7-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="bf2b7-105">Представляет службы Outlook, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="bf2b7-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="bf2b7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bf2b7-106">Methods</span></span>

| <span data-ttu-id="bf2b7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bf2b7-107">Method</span></span>           | <span data-ttu-id="bf2b7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf2b7-108">Return Type</span></span>    |<span data-ttu-id="bf2b7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2b7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf2b7-110">Создание категории</span><span class="sxs-lookup"><span data-stu-id="bf2b7-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="bf2b7-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bf2b7-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="bf2b7-112">Создание объекта **outlookCategory** в основном списке категорий пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf2b7-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="bf2b7-113">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="bf2b7-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="bf2b7-114">Коллекция [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bf2b7-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="bf2b7-115">Получение всех категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf2b7-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="bf2b7-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="bf2b7-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="bf2b7-117">Коллекция [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="bf2b7-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="bf2b7-118">Получение списка языковых стандартов и языков, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf2b7-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="bf2b7-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="bf2b7-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="bf2b7-120">Коллекция [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="bf2b7-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="bf2b7-121">Получение списка часовых поясов, который поддерживается для пользователя, в соответствии с настройкой на сервере почтовых ящиков этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf2b7-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="bf2b7-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf2b7-122">Properties</span></span>
<span data-ttu-id="bf2b7-123">Нет</span><span class="sxs-lookup"><span data-stu-id="bf2b7-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bf2b7-124">Связи</span><span class="sxs-lookup"><span data-stu-id="bf2b7-124">Relationships</span></span>
| <span data-ttu-id="bf2b7-125">Связь</span><span class="sxs-lookup"><span data-stu-id="bf2b7-125">Relationship</span></span> | <span data-ttu-id="bf2b7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="bf2b7-126">Type</span></span>   |<span data-ttu-id="bf2b7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bf2b7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf2b7-128">masterCategories</span><span class="sxs-lookup"><span data-stu-id="bf2b7-128">masterCategories</span></span>|<span data-ttu-id="bf2b7-129">Коллекция [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bf2b7-129">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="bf2b7-130">Список категорий, определенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf2b7-130">A list of categories defined for the user.</span></span> | 

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

