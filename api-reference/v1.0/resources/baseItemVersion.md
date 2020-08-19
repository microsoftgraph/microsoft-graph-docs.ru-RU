---
title: Тип ресурса baseItemVersion
description: Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cc432af84b67e1781be4193a3e8d2bba29ff67a7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808293"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="37867-103">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="37867-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="37867-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37867-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37867-105">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="37867-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="37867-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="37867-106">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="37867-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="37867-107">Properties</span></span>

|      <span data-ttu-id="37867-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="37867-108">Property name</span></span>       |                         <span data-ttu-id="37867-109">Тип</span><span class="sxs-lookup"><span data-stu-id="37867-109">Type</span></span>                         |                               <span data-ttu-id="37867-110">Описание</span><span class="sxs-lookup"><span data-stu-id="37867-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="37867-111">**id**</span><span class="sxs-lookup"><span data-stu-id="37867-111">**id**</span></span>                   | <span data-ttu-id="37867-112">string</span><span class="sxs-lookup"><span data-stu-id="37867-112">string</span></span>                                               | <span data-ttu-id="37867-113">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="37867-113">The ID of the version.</span></span> <span data-ttu-id="37867-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37867-114">Read-only.</span></span>                                       |
| <span data-ttu-id="37867-115">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="37867-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="37867-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="37867-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="37867-117">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="37867-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="37867-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37867-118">Read-only.</span></span>        |
| <span data-ttu-id="37867-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="37867-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="37867-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37867-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="37867-121">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="37867-121">Date and time the version was last modified.</span></span> <span data-ttu-id="37867-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37867-122">Read-only.</span></span>                 |
| <span data-ttu-id="37867-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="37867-123">**publication**</span></span>          | [<span data-ttu-id="37867-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="37867-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="37867-125">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="37867-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="37867-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37867-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
