---
title: Тип ресурса baseItemVersion
description: Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6d74356e20bcc634f2ce9c5e943aa8a53e5f4242
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532016"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="b468d-103">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="b468d-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="b468d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b468d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b468d-105">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="b468d-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b468d-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b468d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b468d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b468d-107">Properties</span></span>

|      <span data-ttu-id="b468d-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b468d-108">Property name</span></span>       |                         <span data-ttu-id="b468d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b468d-109">Type</span></span>                         |                               <span data-ttu-id="b468d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b468d-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="b468d-111">**id**</span><span class="sxs-lookup"><span data-stu-id="b468d-111">**id**</span></span>                   | <span data-ttu-id="b468d-112">string</span><span class="sxs-lookup"><span data-stu-id="b468d-112">string</span></span>                                               | <span data-ttu-id="b468d-113">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="b468d-113">The ID of the version.</span></span> <span data-ttu-id="b468d-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b468d-114">Read-only.</span></span>                                       |
| <span data-ttu-id="b468d-115">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="b468d-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="b468d-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b468d-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="b468d-117">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="b468d-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="b468d-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b468d-118">Read-only.</span></span>        |
| <span data-ttu-id="b468d-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b468d-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="b468d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b468d-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="b468d-121">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="b468d-121">Date and time the version was last modified.</span></span> <span data-ttu-id="b468d-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b468d-122">Read-only.</span></span>                 |
| <span data-ttu-id="b468d-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="b468d-123">**publication**</span></span>          | [<span data-ttu-id="b468d-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="b468d-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="b468d-125">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="b468d-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="b468d-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b468d-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
