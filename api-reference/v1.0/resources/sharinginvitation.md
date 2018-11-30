---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 75fa8212f77873b86748f6d8f63c8e62c8d6a0ca
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="47c8e-102">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="47c8e-102">SharingInvitation resource type</span></span>

<span data-ttu-id="47c8e-103">Ресурс **SharingInvitation** — это единая структура, объединяющая элементы данных, связанные с приглашениями.</span><span class="sxs-lookup"><span data-stu-id="47c8e-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47c8e-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47c8e-104">JSON representation</span></span>

<span data-ttu-id="47c8e-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="47c8e-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="47c8e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="47c8e-106">Properties</span></span>

| <span data-ttu-id="47c8e-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="47c8e-107">Property Name</span></span>  | <span data-ttu-id="47c8e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="47c8e-108">Type</span></span>                          | <span data-ttu-id="47c8e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="47c8e-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="47c8e-110">email</span><span class="sxs-lookup"><span data-stu-id="47c8e-110">email</span></span>          | <span data-ttu-id="47c8e-111">String</span><span class="sxs-lookup"><span data-stu-id="47c8e-111">String</span></span>                        | <span data-ttu-id="47c8e-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47c8e-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="47c8e-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="47c8e-114">invitedBy</span></span>      | [<span data-ttu-id="47c8e-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="47c8e-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="47c8e-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47c8e-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="47c8e-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="47c8e-118">signInRequired</span></span> | <span data-ttu-id="47c8e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="47c8e-119">Boolean</span></span>                       | <span data-ttu-id="47c8e-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47c8e-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="47c8e-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="47c8e-122">Remarks</span></span> 

<span data-ttu-id="47c8e-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="47c8e-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
