---
author: JeremyKelley
description: Ресурс baseItemVersion представляет предыдущую версию элемента или записи.
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d5265004eac969fa827e5456183180a4c6434f96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974238"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="e022d-103">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="e022d-103">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e022d-104">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="e022d-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e022d-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e022d-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e022d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e022d-106">Properties</span></span>

|      <span data-ttu-id="e022d-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e022d-107">Property name</span></span>       |                         <span data-ttu-id="e022d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e022d-108">Type</span></span>                         |                               <span data-ttu-id="e022d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e022d-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e022d-110">**id**</span><span class="sxs-lookup"><span data-stu-id="e022d-110">**id**</span></span>                   | <span data-ttu-id="e022d-111">string</span><span class="sxs-lookup"><span data-stu-id="e022d-111">string</span></span>                                               | <span data-ttu-id="e022d-112">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="e022d-112">The ID of the version.</span></span> <span data-ttu-id="e022d-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e022d-113">Read-only.</span></span>                                       |
| <span data-ttu-id="e022d-114">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="e022d-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e022d-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e022d-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="e022d-116">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="e022d-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e022d-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e022d-117">Read-only.</span></span>        |
| <span data-ttu-id="e022d-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e022d-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e022d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e022d-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e022d-120">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="e022d-120">Date and time the version was last modified.</span></span> <span data-ttu-id="e022d-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e022d-121">Read-only.</span></span>                 |
| <span data-ttu-id="e022d-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="e022d-122">**publication**</span></span>          | [<span data-ttu-id="e022d-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e022d-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e022d-124">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="e022d-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e022d-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e022d-125">Read-only.</span></span> |


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
