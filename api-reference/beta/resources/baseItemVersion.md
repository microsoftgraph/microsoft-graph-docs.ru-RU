---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 9a5181e9cbc089832e8f73e0b8222ca63b69ca30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894483"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="e641c-102">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="e641c-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="e641c-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e641c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e641c-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e641c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e641c-105">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="e641c-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e641c-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e641c-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e641c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e641c-107">Properties</span></span>

|      <span data-ttu-id="e641c-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e641c-108">Property name</span></span>       |                         <span data-ttu-id="e641c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e641c-109">Type</span></span>                         |                               <span data-ttu-id="e641c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e641c-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e641c-111">**id**</span><span class="sxs-lookup"><span data-stu-id="e641c-111">**id**</span></span>                   | <span data-ttu-id="e641c-112">строка</span><span class="sxs-lookup"><span data-stu-id="e641c-112">string</span></span>                                               | <span data-ttu-id="e641c-113">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="e641c-113">The ID of the version.</span></span> <span data-ttu-id="e641c-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e641c-114">Read-only.</span></span>                                       |
| <span data-ttu-id="e641c-115">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="e641c-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e641c-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e641c-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="e641c-117">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="e641c-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e641c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e641c-118">Read-only.</span></span>        |
| <span data-ttu-id="e641c-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e641c-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e641c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e641c-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e641c-121">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="e641c-121">Date and time the version was last modified.</span></span> <span data-ttu-id="e641c-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e641c-122">Read-only.</span></span>                 |
| <span data-ttu-id="e641c-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="e641c-123">**publication**</span></span>          | [<span data-ttu-id="e641c-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e641c-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e641c-125">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="e641c-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e641c-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e641c-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
