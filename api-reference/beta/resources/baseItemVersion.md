---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
ms.openlocfilehash: dfda19af6057bc1d6e1757d24f6a2c99979a8622
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074808"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="a3c16-102">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="a3c16-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="a3c16-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3c16-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3c16-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3c16-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3c16-105">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="a3c16-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3c16-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a3c16-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a3c16-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3c16-107">Properties</span></span>

|      <span data-ttu-id="a3c16-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a3c16-108">Property name</span></span>       |                         <span data-ttu-id="a3c16-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a3c16-109">Type</span></span>                         |                               <span data-ttu-id="a3c16-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3c16-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="a3c16-111">**id**</span><span class="sxs-lookup"><span data-stu-id="a3c16-111">**id**</span></span>                   | <span data-ttu-id="a3c16-112">строка</span><span class="sxs-lookup"><span data-stu-id="a3c16-112">string</span></span>                                               | <span data-ttu-id="a3c16-113">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="a3c16-113">The ID of the version.</span></span> <span data-ttu-id="a3c16-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3c16-114">Read-only.</span></span>                                       |
| <span data-ttu-id="a3c16-115">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="a3c16-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="a3c16-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="a3c16-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="a3c16-117">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="a3c16-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="a3c16-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3c16-118">Read-only.</span></span>        |
| <span data-ttu-id="a3c16-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a3c16-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="a3c16-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3c16-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="a3c16-121">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="a3c16-121">Date and time the version was last modified.</span></span> <span data-ttu-id="a3c16-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3c16-122">Read-only.</span></span>                 |
| <span data-ttu-id="a3c16-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="a3c16-123">**publication**</span></span>          | [<span data-ttu-id="a3c16-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="a3c16-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="a3c16-125">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="a3c16-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="a3c16-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3c16-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->