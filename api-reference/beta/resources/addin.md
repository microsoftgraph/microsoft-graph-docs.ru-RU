---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 1700f3c6bec06c9f2e7ec6093fccffab443d2b08
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895974"
---
# <a name="addin-resource-type"></a><span data-ttu-id="c77a2-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="c77a2-103">addIn resource type</span></span>

<span data-ttu-id="c77a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c77a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c77a2-105">Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах.</span><span class="sxs-lookup"><span data-stu-id="c77a2-105">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="c77a2-106">Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) надстройки для работы с обработчиками файлов.</span><span class="sxs-lookup"><span data-stu-id="c77a2-106">For example, applications that can render file streams [might configure add-ins](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) for File Handler functionality.</span></span> <span data-ttu-id="c77a2-107">Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документа, над которым работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="c77a2-107">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>

## <a name="properties"></a><span data-ttu-id="c77a2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c77a2-108">Properties</span></span>
| <span data-ttu-id="c77a2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c77a2-109">Property</span></span>     | <span data-ttu-id="c77a2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c77a2-110">Type</span></span>   |<span data-ttu-id="c77a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c77a2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c77a2-112">id</span><span class="sxs-lookup"><span data-stu-id="c77a2-112">id</span></span>|<span data-ttu-id="c77a2-113">кодом</span><span class="sxs-lookup"><span data-stu-id="c77a2-113">guid</span></span>||
|<span data-ttu-id="c77a2-114">properties</span><span class="sxs-lookup"><span data-stu-id="c77a2-114">properties</span></span>|<span data-ttu-id="c77a2-115">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c77a2-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="c77a2-116">type</span><span class="sxs-lookup"><span data-stu-id="c77a2-116">type</span></span>|<span data-ttu-id="c77a2-117">string</span><span class="sxs-lookup"><span data-stu-id="c77a2-117">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="c77a2-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c77a2-118">JSON representation</span></span>

<span data-ttu-id="c77a2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c77a2-119">Here is a JSON representation of the resource.</span></span>

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
