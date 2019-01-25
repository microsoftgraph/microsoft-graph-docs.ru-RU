---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 009dcf77492d8ec77230413dc628076ef0d557fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523395"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="ff8b7-102">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="ff8b7-102">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff8b7-103">Ресурс **SharingInvitation** — это единая структура, объединяющая элементы данных, связанные с приглашениями.</span><span class="sxs-lookup"><span data-stu-id="ff8b7-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff8b7-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff8b7-104">JSON representation</span></span>

<span data-ttu-id="ff8b7-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ff8b7-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a><span data-ttu-id="ff8b7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff8b7-106">Properties</span></span>

| <span data-ttu-id="ff8b7-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ff8b7-107">Property Name</span></span>  | <span data-ttu-id="ff8b7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ff8b7-108">Type</span></span>                          | <span data-ttu-id="ff8b7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ff8b7-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ff8b7-110">email</span><span class="sxs-lookup"><span data-stu-id="ff8b7-110">email</span></span>          | <span data-ttu-id="ff8b7-111">String</span><span class="sxs-lookup"><span data-stu-id="ff8b7-111">String</span></span>                        | <span data-ttu-id="ff8b7-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff8b7-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="ff8b7-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="ff8b7-114">invitedBy</span></span>      | [<span data-ttu-id="ff8b7-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="ff8b7-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="ff8b7-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff8b7-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="ff8b7-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="ff8b7-118">signInRequired</span></span> | <span data-ttu-id="ff8b7-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff8b7-119">Boolean</span></span>                       | <span data-ttu-id="ff8b7-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff8b7-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="ff8b7-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="ff8b7-122">Remarks</span></span> 

<span data-ttu-id="ff8b7-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ff8b7-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinginvitation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
