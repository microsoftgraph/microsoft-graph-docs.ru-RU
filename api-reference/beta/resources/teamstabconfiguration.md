---
title: Тип ресурса Теамстабконфигуратион (Open Type)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 449edfbbd04d0f691d89580829684cbe84b168d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046391"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="a0ce7-103">Тип ресурса Теамстабконфигуратион (Open Type)</span><span class="sxs-lookup"><span data-stu-id="a0ce7-103">teamsTabConfiguration resource type (Open Type)</span></span>

<span data-ttu-id="a0ce7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0ce7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ce7-105">Параметры, определяющие содержимое [вкладки](teamstab.md). При настройке вкладки в интерактивном режиме эти сведения задаются приложением поставщика вкладок.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-105">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="a0ce7-106">Помимо приведенных ниже свойств, некоторые приложения поставщика вкладок задают дополнительные настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-106">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="a0ce7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0ce7-107">Properties</span></span>

|<span data-ttu-id="a0ce7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0ce7-108">Property</span></span>|<span data-ttu-id="a0ce7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a0ce7-109">Type</span></span>|<span data-ttu-id="a0ce7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a0ce7-110">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="a0ce7-111">entityId</span><span class="sxs-lookup"><span data-stu-id="a0ce7-111">entityId</span></span>   |   <span data-ttu-id="a0ce7-112">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-112">string</span></span> |  <span data-ttu-id="a0ce7-113">Идентификатор для сущности, размещенной у поставщика вкладок.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-113">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="a0ce7-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="a0ce7-114">contentUrl</span></span> |   <span data-ttu-id="a0ce7-115">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-115">string</span></span> |  <span data-ttu-id="a0ce7-116">URL-адрес, используемый для отображения содержимого вкладки в Teams.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-116">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="a0ce7-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-117">Required.</span></span>    |
|  <span data-ttu-id="a0ce7-118">removeUrl</span><span class="sxs-lookup"><span data-stu-id="a0ce7-118">removeUrl</span></span>  |   <span data-ttu-id="a0ce7-119">строка</span><span class="sxs-lookup"><span data-stu-id="a0ce7-119">string</span></span> |  <span data-ttu-id="a0ce7-120">URL-адрес, вызываемый клиентом Teams при удалении вкладки с помощью клиента Teams.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-120">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="a0ce7-121">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="a0ce7-121">websiteUrl</span></span> |   <span data-ttu-id="a0ce7-122">string</span><span class="sxs-lookup"><span data-stu-id="a0ce7-122">string</span></span> |  <span data-ttu-id="a0ce7-123">URL-адрес для отображения содержимого вкладки вне Teams.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-123">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="a0ce7-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0ce7-124">JSON representation</span></span>

<span data-ttu-id="a0ce7-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0ce7-125">The following is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


