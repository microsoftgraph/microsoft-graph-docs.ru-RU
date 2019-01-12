---
title: teamsTabConfiguration ресурсов (тип Open)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9873d9e03fec5d7751270b963015aed9eeb0ab48
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953639"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="d931c-103">teamsTabConfiguration ресурсов (тип Open)</span><span class="sxs-lookup"><span data-stu-id="d931c-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="d931c-104">Параметры, определяющие содержимое [вкладки](teamstab.md). Если вкладки интерактивно настроено, эти сведения задается приложение поставщика вкладки.</span><span class="sxs-lookup"><span data-stu-id="d931c-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="d931c-105">В дополнение к указанные ниже свойства некоторые приложения поставщика вкладки укажите дополнительные настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="d931c-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="d931c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d931c-106">Properties</span></span>

|<span data-ttu-id="d931c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d931c-107">Property</span></span>|<span data-ttu-id="d931c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d931c-108">Type</span></span>|<span data-ttu-id="d931c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d931c-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="d931c-110">entityId</span><span class="sxs-lookup"><span data-stu-id="d931c-110">entityId</span></span>   |   <span data-ttu-id="d931c-111">строка</span><span class="sxs-lookup"><span data-stu-id="d931c-111">string</span></span> |  <span data-ttu-id="d931c-112">Идентификатор для сущности, размещенного поставщиком вкладки.</span><span class="sxs-lookup"><span data-stu-id="d931c-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="d931c-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="d931c-113">contentUrl</span></span> |   <span data-ttu-id="d931c-114">строка</span><span class="sxs-lookup"><span data-stu-id="d931c-114">string</span></span> |  <span data-ttu-id="d931c-115">URL-адрес, используемый для отображения содержимого вкладки в группах.</span><span class="sxs-lookup"><span data-stu-id="d931c-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="d931c-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d931c-116">Required.</span></span>    |
|  <span data-ttu-id="d931c-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="d931c-117">removeUrl</span></span>  |   <span data-ttu-id="d931c-118">строка</span><span class="sxs-lookup"><span data-stu-id="d931c-118">string</span></span> |  <span data-ttu-id="d931c-119">URL-адрес, вызванный клиентом команды при удалении вкладки с помощью команды клиента.</span><span class="sxs-lookup"><span data-stu-id="d931c-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="d931c-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="d931c-120">websiteUrl</span></span> |   <span data-ttu-id="d931c-121">строка</span><span class="sxs-lookup"><span data-stu-id="d931c-121">string</span></span> |  <span data-ttu-id="d931c-122">URL-адрес для отображения содержимого вкладки вне группы.</span><span class="sxs-lookup"><span data-stu-id="d931c-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="d931c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d931c-123">JSON representation</span></span>

<span data-ttu-id="d931c-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d931c-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
