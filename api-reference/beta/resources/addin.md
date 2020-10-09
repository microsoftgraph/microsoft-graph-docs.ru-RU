---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: cd638480c6e05413b20dad389257bf9a43174e40
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405633"
---
# <a name="addin-resource-type"></a><span data-ttu-id="18090-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="18090-103">addIn resource type</span></span>

<span data-ttu-id="18090-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18090-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18090-105">Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="18090-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="18090-106">Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать](/onedrive/developer/file-handlers/?view=odsp-graph-online) надстройки для работы с обработчиками файлов.</span><span class="sxs-lookup"><span data-stu-id="18090-106">For example, applications that can render file streams [might configure add-ins](/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="18090-107">Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="18090-107">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="18090-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="18090-108">Properties</span></span>
| <span data-ttu-id="18090-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="18090-109">Property</span></span>     | <span data-ttu-id="18090-110">Тип</span><span class="sxs-lookup"><span data-stu-id="18090-110">Type</span></span>   |<span data-ttu-id="18090-111">Описание</span><span class="sxs-lookup"><span data-stu-id="18090-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18090-112">id</span><span class="sxs-lookup"><span data-stu-id="18090-112">id</span></span>|<span data-ttu-id="18090-113">кодом</span><span class="sxs-lookup"><span data-stu-id="18090-113">guid</span></span>||
|<span data-ttu-id="18090-114">properties</span><span class="sxs-lookup"><span data-stu-id="18090-114">properties</span></span>|<span data-ttu-id="18090-115">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="18090-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="18090-116">type</span><span class="sxs-lookup"><span data-stu-id="18090-116">type</span></span>|<span data-ttu-id="18090-117">string</span><span class="sxs-lookup"><span data-stu-id="18090-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="18090-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18090-118">JSON representation</span></span>

<span data-ttu-id="18090-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18090-119">Here is a JSON representation of the resource.</span></span>

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