---
author: JeremyKelley
description: Ресурс baseItemVersion представляет предыдущую версию элемента или записи.
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 47865e388616763b60ce3cd45195bf9919c7acf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508040"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="f6545-103">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="f6545-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="f6545-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6545-105">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="f6545-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f6545-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f6545-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="f6545-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6545-107">Properties</span></span>

|      <span data-ttu-id="f6545-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f6545-108">Property name</span></span>       |                         <span data-ttu-id="f6545-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6545-109">Type</span></span>                         |                               <span data-ttu-id="f6545-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6545-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="f6545-111">**id**</span><span class="sxs-lookup"><span data-stu-id="f6545-111">**id**</span></span>                   | <span data-ttu-id="f6545-112">string</span><span class="sxs-lookup"><span data-stu-id="f6545-112">string</span></span>                                               | <span data-ttu-id="f6545-113">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="f6545-113">The ID of the version.</span></span> <span data-ttu-id="f6545-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6545-114">Read-only.</span></span>                                       |
| <span data-ttu-id="f6545-115">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="f6545-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="f6545-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f6545-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="f6545-117">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="f6545-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="f6545-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6545-118">Read-only.</span></span>        |
| <span data-ttu-id="f6545-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f6545-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="f6545-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6545-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="f6545-121">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="f6545-121">Date and time the version was last modified.</span></span> <span data-ttu-id="f6545-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6545-122">Read-only.</span></span>                 |
| <span data-ttu-id="f6545-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="f6545-123">**publication**</span></span>          | [<span data-ttu-id="f6545-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="f6545-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="f6545-125">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="f6545-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="f6545-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6545-126">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
