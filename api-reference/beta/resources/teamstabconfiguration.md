---
title: teamsTabConfiguration ресурсов (тип Open)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 10cc22e70288d1643a3a2cdebe23a012e22e3879
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519201"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="ce3c3-103">teamsTabConfiguration ресурсов (тип Open)</span><span class="sxs-lookup"><span data-stu-id="ce3c3-103">teamsTabConfiguration resource type (Open Type)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce3c3-104">Параметры, определяющие содержимое [вкладки](teamstab.md). Если вкладки интерактивно настроено, эти сведения задается приложение поставщика вкладки.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-104">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="ce3c3-105">В дополнение к указанные ниже свойства некоторые приложения поставщика вкладки укажите дополнительные настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-105">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="ce3c3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce3c3-106">Properties</span></span>

|<span data-ttu-id="ce3c3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce3c3-107">Property</span></span>|<span data-ttu-id="ce3c3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ce3c3-108">Type</span></span>|<span data-ttu-id="ce3c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce3c3-109">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="ce3c3-110">entityId</span><span class="sxs-lookup"><span data-stu-id="ce3c3-110">entityId</span></span>   |   <span data-ttu-id="ce3c3-111">string</span><span class="sxs-lookup"><span data-stu-id="ce3c3-111">string</span></span> |  <span data-ttu-id="ce3c3-112">Идентификатор для сущности, размещенного поставщиком вкладки.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-112">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="ce3c3-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="ce3c3-113">contentUrl</span></span> |   <span data-ttu-id="ce3c3-114">string</span><span class="sxs-lookup"><span data-stu-id="ce3c3-114">string</span></span> |  <span data-ttu-id="ce3c3-115">URL-адрес, используемый для отображения содержимого вкладки в группах.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-115">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="ce3c3-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-116">Required.</span></span>    |
|  <span data-ttu-id="ce3c3-117">removeUrl</span><span class="sxs-lookup"><span data-stu-id="ce3c3-117">removeUrl</span></span>  |   <span data-ttu-id="ce3c3-118">string</span><span class="sxs-lookup"><span data-stu-id="ce3c3-118">string</span></span> |  <span data-ttu-id="ce3c3-119">URL-адрес, вызванный клиентом команды при удалении вкладки с помощью команды клиента.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-119">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="ce3c3-120">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="ce3c3-120">websiteUrl</span></span> |   <span data-ttu-id="ce3c3-121">string</span><span class="sxs-lookup"><span data-stu-id="ce3c3-121">string</span></span> |  <span data-ttu-id="ce3c3-122">URL-адрес для отображения содержимого вкладки вне группы.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-122">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="ce3c3-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce3c3-123">JSON representation</span></span>

<span data-ttu-id="ce3c3-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce3c3-124">The following is a JSON representation of the resource.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstabconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
