---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 187a7bd8fe51be57b663c215436272ee711512e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026283"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="8fc6c-102">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="8fc6c-102">SharingInvitation resource type</span></span>

<span data-ttu-id="8fc6c-103">Ресурс **SharingInvitation** группирует элементы данных, связанных с приглашением в одной структуры.</span><span class="sxs-lookup"><span data-stu-id="8fc6c-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fc6c-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fc6c-104">JSON representation</span></span>

<span data-ttu-id="8fc6c-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fc6c-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8fc6c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fc6c-106">Properties</span></span>

| <span data-ttu-id="8fc6c-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8fc6c-107">Property Name</span></span>  | <span data-ttu-id="8fc6c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8fc6c-108">Type</span></span>            | <span data-ttu-id="8fc6c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8fc6c-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="8fc6c-110">email</span><span class="sxs-lookup"><span data-stu-id="8fc6c-110">email</span></span>          | <span data-ttu-id="8fc6c-111">String</span><span class="sxs-lookup"><span data-stu-id="8fc6c-111">String</span></span>          | <span data-ttu-id="8fc6c-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fc6c-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="8fc6c-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="8fc6c-114">invitedBy</span></span>      | <span data-ttu-id="8fc6c-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8fc6c-115">[identitySet][]</span></span> | <span data-ttu-id="8fc6c-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fc6c-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="8fc6c-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="8fc6c-118">signInRequired</span></span> | <span data-ttu-id="8fc6c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fc6c-119">Boolean</span></span>         | <span data-ttu-id="8fc6c-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fc6c-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="8fc6c-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="8fc6c-122">Remarks</span></span>

<span data-ttu-id="8fc6c-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8fc6c-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
