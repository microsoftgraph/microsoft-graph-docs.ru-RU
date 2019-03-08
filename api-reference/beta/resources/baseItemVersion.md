---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 56a2c230c53c4b5bd50e8c123dd69eedec67a141
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480672"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="7ddbe-102">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="7ddbe-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ddbe-103">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7ddbe-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7ddbe-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7ddbe-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ddbe-105">Properties</span></span>

|      <span data-ttu-id="7ddbe-106">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7ddbe-106">Property name</span></span>       |                         <span data-ttu-id="7ddbe-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7ddbe-107">Type</span></span>                         |                               <span data-ttu-id="7ddbe-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7ddbe-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="7ddbe-109">**id**</span><span class="sxs-lookup"><span data-stu-id="7ddbe-109">**id**</span></span>                   | <span data-ttu-id="7ddbe-110">string</span><span class="sxs-lookup"><span data-stu-id="7ddbe-110">string</span></span>                                               | <span data-ttu-id="7ddbe-111">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-111">The ID of the version.</span></span> <span data-ttu-id="7ddbe-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-112">Read-only.</span></span>                                       |
| <span data-ttu-id="7ddbe-113">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="7ddbe-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="7ddbe-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="7ddbe-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="7ddbe-115">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="7ddbe-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-116">Read-only.</span></span>        |
| <span data-ttu-id="7ddbe-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7ddbe-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="7ddbe-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ddbe-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="7ddbe-119">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-119">Date and time the version was last modified.</span></span> <span data-ttu-id="7ddbe-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-120">Read-only.</span></span>                 |
| <span data-ttu-id="7ddbe-121">**publication**</span><span class="sxs-lookup"><span data-stu-id="7ddbe-121">**publication**</span></span>          | [<span data-ttu-id="7ddbe-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="7ddbe-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="7ddbe-123">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="7ddbe-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ddbe-124">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
