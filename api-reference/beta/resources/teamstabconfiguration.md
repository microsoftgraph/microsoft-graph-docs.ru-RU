---
title: teamsTabConfiguration ресурсов (тип Open)
description: Параметры, определяющие содержимое вкладки.
author: nkramer
ms.openlocfilehash: 9abb4e9089da760825b29c4001b68881ab74d815
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301185"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="63f06-103">teamsTabConfiguration ресурсов (тип Open)</span><span class="sxs-lookup"><span data-stu-id="63f06-103">teamsTabConfiguration resource type (Open Type)</span></span>

> <span data-ttu-id="63f06-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="63f06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63f06-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63f06-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63f06-106">Параметры, определяющие содержимое [вкладки](teamstab.md). Если вкладки интерактивно настроено, эти сведения задается приложение поставщика вкладки.</span><span class="sxs-lookup"><span data-stu-id="63f06-106">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="63f06-107">В дополнение к указанные ниже свойства некоторые приложения поставщика вкладки укажите дополнительные настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="63f06-107">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="63f06-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="63f06-108">Properties</span></span>

|<span data-ttu-id="63f06-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="63f06-109">Property</span></span>|<span data-ttu-id="63f06-110">Тип</span><span class="sxs-lookup"><span data-stu-id="63f06-110">Type</span></span>|<span data-ttu-id="63f06-111">Описание</span><span class="sxs-lookup"><span data-stu-id="63f06-111">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="63f06-112">entityId</span><span class="sxs-lookup"><span data-stu-id="63f06-112">entityId</span></span>   |   <span data-ttu-id="63f06-113">строка</span><span class="sxs-lookup"><span data-stu-id="63f06-113">string</span></span> |  <span data-ttu-id="63f06-114">Идентификатор для сущности, размещенного поставщиком вкладки.</span><span class="sxs-lookup"><span data-stu-id="63f06-114">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="63f06-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="63f06-115">contentUrl</span></span> |   <span data-ttu-id="63f06-116">строка</span><span class="sxs-lookup"><span data-stu-id="63f06-116">string</span></span> |  <span data-ttu-id="63f06-117">URL-адрес, используемый для отображения содержимого вкладки в группах.</span><span class="sxs-lookup"><span data-stu-id="63f06-117">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="63f06-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63f06-118">Required.</span></span>    |
|  <span data-ttu-id="63f06-119">removeUrl</span><span class="sxs-lookup"><span data-stu-id="63f06-119">removeUrl</span></span>  |   <span data-ttu-id="63f06-120">строка</span><span class="sxs-lookup"><span data-stu-id="63f06-120">string</span></span> |  <span data-ttu-id="63f06-121">URL-адрес, вызванный клиентом команды при удалении вкладки с помощью команды клиента.</span><span class="sxs-lookup"><span data-stu-id="63f06-121">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="63f06-122">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="63f06-122">websiteUrl</span></span> |   <span data-ttu-id="63f06-123">строка</span><span class="sxs-lookup"><span data-stu-id="63f06-123">string</span></span> |  <span data-ttu-id="63f06-124">URL-адрес для отображения содержимого вкладки вне группы.</span><span class="sxs-lookup"><span data-stu-id="63f06-124">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="63f06-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63f06-125">JSON representation</span></span>

<span data-ttu-id="63f06-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63f06-126">The following is a JSON representation of the resource.</span></span>
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
