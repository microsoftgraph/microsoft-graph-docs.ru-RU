---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 136f35bc47e304a8dc844a9ee4ac86cd49c8928f
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639159"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="12150-102">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="12150-102">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12150-103">Ресурс **SharingInvitation** группирует элементы данных, связанные с приглашением, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="12150-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12150-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12150-104">JSON representation</span></span>

<span data-ttu-id="12150-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="12150-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="12150-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="12150-106">Properties</span></span>

| <span data-ttu-id="12150-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="12150-107">Property Name</span></span>  | <span data-ttu-id="12150-108">Тип</span><span class="sxs-lookup"><span data-stu-id="12150-108">Type</span></span>                          | <span data-ttu-id="12150-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12150-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="12150-110">email</span><span class="sxs-lookup"><span data-stu-id="12150-110">email</span></span>          | <span data-ttu-id="12150-111">String</span><span class="sxs-lookup"><span data-stu-id="12150-111">String</span></span>                        | <span data-ttu-id="12150-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12150-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="12150-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="12150-114">invitedBy</span></span>      | [<span data-ttu-id="12150-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="12150-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="12150-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12150-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="12150-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="12150-118">signInRequired</span></span> | <span data-ttu-id="12150-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="12150-119">Boolean</span></span>                       | <span data-ttu-id="12150-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12150-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="12150-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="12150-122">Remarks</span></span> 

<span data-ttu-id="12150-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="12150-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
