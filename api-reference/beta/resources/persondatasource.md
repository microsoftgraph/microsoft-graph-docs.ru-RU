---
title: Тип ресурса personDataSource
description: Представляет источников, которые пользователь данные извлекаются из, например, каталогов и контактов Outlook.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 540ffa81b20b40f9df2694ba634777250742daaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978503"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="6bb13-103">Тип ресурса personDataSource</span><span class="sxs-lookup"><span data-stu-id="6bb13-103">personDataSource resource type</span></span>

> <span data-ttu-id="6bb13-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6bb13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bb13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bb13-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6bb13-106">Представляет источников, которые пользователь данные извлекаются из, например, каталогов и контактов Outlook.</span><span class="sxs-lookup"><span data-stu-id="6bb13-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bb13-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bb13-107">JSON representation</span></span>

<span data-ttu-id="6bb13-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6bb13-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="6bb13-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bb13-109">Properties</span></span>
| <span data-ttu-id="6bb13-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bb13-110">Property</span></span>     | <span data-ttu-id="6bb13-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6bb13-111">Type</span></span>   |<span data-ttu-id="6bb13-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6bb13-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bb13-113">type</span><span class="sxs-lookup"><span data-stu-id="6bb13-113">type</span></span>|<span data-ttu-id="6bb13-114">Строка</span><span class="sxs-lookup"><span data-stu-id="6bb13-114">String</span></span>|<span data-ttu-id="6bb13-115">Тип источника данных.</span><span class="sxs-lookup"><span data-stu-id="6bb13-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
