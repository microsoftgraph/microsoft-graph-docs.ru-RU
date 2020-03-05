---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a5f0d078bf73603ccedf905c2cd496223fbd426e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508417"
---
# <a name="addin-resource-type"></a><span data-ttu-id="d66be-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="d66be-103">addIn resource type</span></span>

<span data-ttu-id="d66be-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d66be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d66be-105">Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="d66be-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="d66be-106">Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) надстройки для работы с обработчиками файлов.</span><span class="sxs-lookup"><span data-stu-id="d66be-106">For example, applications that can render file streams [might configure add-ins](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="d66be-107">Это позволит таким службам, как Office 365, вызывать приложение в контексте документов, над которыми работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="d66be-107">This will let services like Office 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="d66be-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d66be-108">Properties</span></span>
| <span data-ttu-id="d66be-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d66be-109">Property</span></span>     | <span data-ttu-id="d66be-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d66be-110">Type</span></span>   |<span data-ttu-id="d66be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d66be-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d66be-112">id</span><span class="sxs-lookup"><span data-stu-id="d66be-112">id</span></span>|<span data-ttu-id="d66be-113">кодом</span><span class="sxs-lookup"><span data-stu-id="d66be-113">guid</span></span>||
|<span data-ttu-id="d66be-114">properties</span><span class="sxs-lookup"><span data-stu-id="d66be-114">properties</span></span>|<span data-ttu-id="d66be-115">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d66be-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="d66be-116">type</span><span class="sxs-lookup"><span data-stu-id="d66be-116">type</span></span>|<span data-ttu-id="d66be-117">string</span><span class="sxs-lookup"><span data-stu-id="d66be-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="d66be-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d66be-118">JSON representation</span></span>

<span data-ttu-id="d66be-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d66be-119">Here is a JSON representation of the resource.</span></span>

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
