---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 3671ad561fde44aac90d20284c7acbfedba6b0c3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863937"
---
# <a name="addin-resource-type"></a><span data-ttu-id="8967a-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="8967a-103">addIn resource type</span></span>

<span data-ttu-id="8967a-104">Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="8967a-104">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="8967a-105">Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать надстройки](/onedrive/developer/file-handlers/?view=odsp-graph-online) для своей функции "филехандлер".</span><span class="sxs-lookup"><span data-stu-id="8967a-105">For example, applications that can render file streams [may configure addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="8967a-106">Это позволит таким службам, как Office 365, вызывать приложение в контексте документов, над которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="8967a-106">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="8967a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8967a-107">Properties</span></span>
| <span data-ttu-id="8967a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8967a-108">Property</span></span>     | <span data-ttu-id="8967a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8967a-109">Type</span></span>   |<span data-ttu-id="8967a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8967a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8967a-111">id</span><span class="sxs-lookup"><span data-stu-id="8967a-111">id</span></span>|<span data-ttu-id="8967a-112">кодом</span><span class="sxs-lookup"><span data-stu-id="8967a-112">guid</span></span>||
|<span data-ttu-id="8967a-113">properties</span><span class="sxs-lookup"><span data-stu-id="8967a-113">properties</span></span>|<span data-ttu-id="8967a-114">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8967a-114">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="8967a-115">type</span><span class="sxs-lookup"><span data-stu-id="8967a-115">type</span></span>|<span data-ttu-id="8967a-116">string</span><span class="sxs-lookup"><span data-stu-id="8967a-116">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="8967a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8967a-117">JSON representation</span></span>

<span data-ttu-id="8967a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8967a-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
