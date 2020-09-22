---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: bbb7a106c3710b5f7e433bfe0c7904f9df91a988
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988592"
---
# <a name="addin-resource-type"></a><span data-ttu-id="4c7de-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="4c7de-103">addIn resource type</span></span>

<span data-ttu-id="4c7de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c7de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c7de-105">Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="4c7de-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="4c7de-106">Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать надстройки](/onedrive/developer/file-handlers/?view=odsp-graph-online) для своей функции "филехандлер".</span><span class="sxs-lookup"><span data-stu-id="4c7de-106">For example, applications that can render file streams [may configure addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="4c7de-107">Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="4c7de-107">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="4c7de-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c7de-108">Properties</span></span>
| <span data-ttu-id="4c7de-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c7de-109">Property</span></span>     | <span data-ttu-id="4c7de-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4c7de-110">Type</span></span>   |<span data-ttu-id="4c7de-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4c7de-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c7de-112">id</span><span class="sxs-lookup"><span data-stu-id="4c7de-112">id</span></span>|<span data-ttu-id="4c7de-113">кодом</span><span class="sxs-lookup"><span data-stu-id="4c7de-113">guid</span></span>||
|<span data-ttu-id="4c7de-114">properties</span><span class="sxs-lookup"><span data-stu-id="4c7de-114">properties</span></span>|<span data-ttu-id="4c7de-115">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4c7de-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="4c7de-116">type</span><span class="sxs-lookup"><span data-stu-id="4c7de-116">type</span></span>|<span data-ttu-id="4c7de-117">string</span><span class="sxs-lookup"><span data-stu-id="4c7de-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="4c7de-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c7de-118">JSON representation</span></span>

<span data-ttu-id="4c7de-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c7de-119">Here is a JSON representation of the resource.</span></span>

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

