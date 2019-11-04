---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 26a224989af3ab87036fbd6bd0964ea811016dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939097"
---
# <a name="addin-resource-type"></a><span data-ttu-id="e9ec6-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="e9ec6-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9ec6-104">Определяет пользовательское поведение, которое может использоваться службой использования для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="e9ec6-104">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="e9ec6-105">Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) надстройки для работы с обработчиками файлов.</span><span class="sxs-lookup"><span data-stu-id="e9ec6-105">For example, applications that can render file streams [might configure add-ins](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="e9ec6-106">Это позволит таким службам, как Office 365, вызвать приложение в контексте документа, над которым работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="e9ec6-106">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="e9ec6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9ec6-107">Properties</span></span>
| <span data-ttu-id="e9ec6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9ec6-108">Property</span></span>     | <span data-ttu-id="e9ec6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e9ec6-109">Type</span></span>   |<span data-ttu-id="e9ec6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e9ec6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9ec6-111">id</span><span class="sxs-lookup"><span data-stu-id="e9ec6-111">id</span></span>|<span data-ttu-id="e9ec6-112">кодом</span><span class="sxs-lookup"><span data-stu-id="e9ec6-112">guid</span></span>||
|<span data-ttu-id="e9ec6-113">properties</span><span class="sxs-lookup"><span data-stu-id="e9ec6-113">properties</span></span>|<span data-ttu-id="e9ec6-114">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e9ec6-114">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="e9ec6-115">type</span><span class="sxs-lookup"><span data-stu-id="e9ec6-115">type</span></span>|<span data-ttu-id="e9ec6-116">string</span><span class="sxs-lookup"><span data-stu-id="e9ec6-116">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="e9ec6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9ec6-117">JSON representation</span></span>

<span data-ttu-id="e9ec6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9ec6-118">Here is a JSON representation of the resource.</span></span>

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
