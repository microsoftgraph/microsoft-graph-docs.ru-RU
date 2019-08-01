---
title: Тип ресурса Теамстабконфигуратион (Open Type)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a3c16c69acefb8f746d11807a898e74de7620be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033686"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="50cd9-103">Тип ресурса Теамстабконфигуратион (Open Type)</span><span class="sxs-lookup"><span data-stu-id="50cd9-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="50cd9-104">Параметры, определяющие содержимое [вкладки](teamstab.md). При настройке вкладки в интерактивном режиме эти сведения задаются приложением поставщика вкладок.</span><span class="sxs-lookup"><span data-stu-id="50cd9-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="50cd9-105">Помимо приведенных ниже свойств, некоторые приложения поставщика вкладок задают дополнительные настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="50cd9-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="50cd9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="50cd9-106">Properties</span></span>

|<span data-ttu-id="50cd9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="50cd9-107">Property</span></span>|<span data-ttu-id="50cd9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="50cd9-108">Type</span></span>|<span data-ttu-id="50cd9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="50cd9-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="50cd9-110">entityId</span><span class="sxs-lookup"><span data-stu-id="50cd9-110">entityId</span></span>   |   <span data-ttu-id="50cd9-111">string</span><span class="sxs-lookup"><span data-stu-id="50cd9-111">string</span></span> |  <span data-ttu-id="50cd9-112">Идентификатор для сущности, размещенной у поставщика вкладок.</span><span class="sxs-lookup"><span data-stu-id="50cd9-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="50cd9-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="50cd9-113">contentUrl</span></span> |   <span data-ttu-id="50cd9-114">string</span><span class="sxs-lookup"><span data-stu-id="50cd9-114">string</span></span> |  <span data-ttu-id="50cd9-115">URL-адрес, используемый для отображения содержимого вкладки в Teams.</span><span class="sxs-lookup"><span data-stu-id="50cd9-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="50cd9-116">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="50cd9-116">Required.</span></span>    |
|  <span data-ttu-id="50cd9-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="50cd9-117">removeUrl</span></span>  |   <span data-ttu-id="50cd9-118">string</span><span class="sxs-lookup"><span data-stu-id="50cd9-118">string</span></span> |  <span data-ttu-id="50cd9-119">URL-адрес, вызываемый клиентом Teams при удалении вкладки с помощью клиента Teams.</span><span class="sxs-lookup"><span data-stu-id="50cd9-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="50cd9-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="50cd9-120">websiteUrl</span></span> |   <span data-ttu-id="50cd9-121">string</span><span class="sxs-lookup"><span data-stu-id="50cd9-121">string</span></span> |  <span data-ttu-id="50cd9-122">URL-адрес для отображения содержимого вкладки вне Teams.</span><span class="sxs-lookup"><span data-stu-id="50cd9-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="50cd9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50cd9-123">JSON representation</span></span>

<span data-ttu-id="50cd9-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50cd9-124">The following is a JSON representation of the resource.</span></span>
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
