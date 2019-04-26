---
title: Тип ресурса Теамстабконфигуратион (Open Type)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: beeb9c6b06457795b802e18a1a2f7fac909e0c6c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345734"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="31aa5-103">Тип ресурса Теамстабконфигуратион (Open Type)</span><span class="sxs-lookup"><span data-stu-id="31aa5-103">teamsTabConfiguration resource type (Open Type)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31aa5-104">Параметры, определяющие содержимое [вкладки](teamstab.md). При настройке вкладки в интерактивном режиме эти сведения задаются приложением поставщика вкладок.</span><span class="sxs-lookup"><span data-stu-id="31aa5-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="31aa5-105">Помимо приведенных ниже свойств, некоторые приложения поставщика вкладок задают дополнительные настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="31aa5-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="31aa5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="31aa5-106">Properties</span></span>

|<span data-ttu-id="31aa5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="31aa5-107">Property</span></span>|<span data-ttu-id="31aa5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="31aa5-108">Type</span></span>|<span data-ttu-id="31aa5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="31aa5-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="31aa5-110">entityId</span><span class="sxs-lookup"><span data-stu-id="31aa5-110">entityId</span></span>   |   <span data-ttu-id="31aa5-111">строка</span><span class="sxs-lookup"><span data-stu-id="31aa5-111">string</span></span> |  <span data-ttu-id="31aa5-112">Идентификатор для сущности, размещенной у поставщика вкладок.</span><span class="sxs-lookup"><span data-stu-id="31aa5-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="31aa5-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="31aa5-113">contentUrl</span></span> |   <span data-ttu-id="31aa5-114">строка</span><span class="sxs-lookup"><span data-stu-id="31aa5-114">string</span></span> |  <span data-ttu-id="31aa5-115">URL-адрес, используемый для отображения содержимого вкладки в Teams.</span><span class="sxs-lookup"><span data-stu-id="31aa5-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="31aa5-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31aa5-116">Required.</span></span>    |
|  <span data-ttu-id="31aa5-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="31aa5-117">removeUrl</span></span>  |   <span data-ttu-id="31aa5-118">строка</span><span class="sxs-lookup"><span data-stu-id="31aa5-118">string</span></span> |  <span data-ttu-id="31aa5-119">URL-адрес, вызываемый клиентом Teams при удалении вкладки с помощью клиента Teams.</span><span class="sxs-lookup"><span data-stu-id="31aa5-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="31aa5-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="31aa5-120">websiteUrl</span></span> |   <span data-ttu-id="31aa5-121">string</span><span class="sxs-lookup"><span data-stu-id="31aa5-121">string</span></span> |  <span data-ttu-id="31aa5-122">URL-адрес для отображения содержимого вкладки вне Teams.</span><span class="sxs-lookup"><span data-stu-id="31aa5-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="31aa5-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="31aa5-123">JSON representation</span></span>

<span data-ttu-id="31aa5-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31aa5-124">The following is a JSON representation of the resource.</span></span>
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
