---
title: teamsTabConfiguration ресурсов (тип Open)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c33ab6d5102498ab26fcc609328c2562707883d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858473"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="0e0f3-103">teamsTabConfiguration ресурсов (тип Open)</span><span class="sxs-lookup"><span data-stu-id="0e0f3-103">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="0e0f3-104">Параметры, определяющие содержимое [вкладки](teamstab.md). Если вкладки интерактивно настроено, эти сведения задается приложение поставщика вкладки.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="0e0f3-105">В дополнение к указанные ниже свойства некоторые приложения поставщика вкладки укажите дополнительные настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="0e0f3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e0f3-106">Properties</span></span>

|<span data-ttu-id="0e0f3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e0f3-107">Property</span></span>|<span data-ttu-id="0e0f3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0e0f3-108">Type</span></span>|<span data-ttu-id="0e0f3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0e0f3-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="0e0f3-110">entityId</span><span class="sxs-lookup"><span data-stu-id="0e0f3-110">entityId</span></span>   |   <span data-ttu-id="0e0f3-111">строка</span><span class="sxs-lookup"><span data-stu-id="0e0f3-111">string</span></span> |  <span data-ttu-id="0e0f3-112">Идентификатор для сущности, размещенного поставщиком вкладки.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="0e0f3-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0e0f3-113">contentUrl</span></span> |   <span data-ttu-id="0e0f3-114">строка</span><span class="sxs-lookup"><span data-stu-id="0e0f3-114">string</span></span> |  <span data-ttu-id="0e0f3-115">URL-адрес, используемый для отображения содержимого вкладки в группах.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="0e0f3-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-116">Required.</span></span>    |
|  <span data-ttu-id="0e0f3-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="0e0f3-117">removeUrl</span></span>  |   <span data-ttu-id="0e0f3-118">строка</span><span class="sxs-lookup"><span data-stu-id="0e0f3-118">string</span></span> |  <span data-ttu-id="0e0f3-119">URL-адрес, вызванный клиентом команды при удалении вкладки с помощью команды клиента.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="0e0f3-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="0e0f3-120">websiteUrl</span></span> |   <span data-ttu-id="0e0f3-121">строка</span><span class="sxs-lookup"><span data-stu-id="0e0f3-121">string</span></span> |  <span data-ttu-id="0e0f3-122">URL-адрес для отображения содержимого вкладки вне группы.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="0e0f3-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e0f3-123">JSON representation</span></span>

<span data-ttu-id="0e0f3-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e0f3-124">The following is a JSON representation of the resource.</span></span>
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
