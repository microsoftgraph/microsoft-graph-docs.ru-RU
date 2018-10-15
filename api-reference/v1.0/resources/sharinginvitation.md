---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 9237c401fd83a7b30303f147402262c022b820a7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265857"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="59291-102">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="59291-102">SharingInvitation resource type</span></span>

<span data-ttu-id="59291-103">Ресурс **SharingInvitation** группирует элементы данных, связанные с приглашениями, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="59291-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59291-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59291-104">JSON representation</span></span>

<span data-ttu-id="59291-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59291-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="59291-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="59291-106">Properties</span></span>

| <span data-ttu-id="59291-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="59291-107">Property Name</span></span>  | <span data-ttu-id="59291-108">Тип</span><span class="sxs-lookup"><span data-stu-id="59291-108">Type</span></span>            | <span data-ttu-id="59291-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59291-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="59291-110">email</span><span class="sxs-lookup"><span data-stu-id="59291-110">email</span></span>          | <span data-ttu-id="59291-111">String (строка)</span><span class="sxs-lookup"><span data-stu-id="59291-111">String</span></span>          | <span data-ttu-id="59291-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59291-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="59291-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="59291-114">invitedBy</span></span>      | <span data-ttu-id="59291-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="59291-115">[identitySet][]</span></span> | <span data-ttu-id="59291-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59291-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="59291-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="59291-118">signInRequired</span></span> | <span data-ttu-id="59291-119">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="59291-119">Boolean</span></span>         | <span data-ttu-id="59291-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59291-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="59291-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="59291-122">Remarks</span></span>

<span data-ttu-id="59291-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="59291-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveItem.md
[IdentitySet]: identitySet.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
