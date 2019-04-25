---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 0cb09136f4093b290f37ee851cb7d2d0ca10c1bf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549596"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="414cf-102">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="414cf-102">SharingInvitation resource type</span></span>

<span data-ttu-id="414cf-103">Ресурс **SharingInvitation** группирует элементы данных, связанные с приглашением, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="414cf-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="414cf-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="414cf-104">JSON representation</span></span>

<span data-ttu-id="414cf-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="414cf-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="414cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="414cf-106">Properties</span></span>

| <span data-ttu-id="414cf-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="414cf-107">Property Name</span></span>  | <span data-ttu-id="414cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="414cf-108">Type</span></span>            | <span data-ttu-id="414cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="414cf-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="414cf-110">email</span><span class="sxs-lookup"><span data-stu-id="414cf-110">email</span></span>          | <span data-ttu-id="414cf-111">String</span><span class="sxs-lookup"><span data-stu-id="414cf-111">String</span></span>          | <span data-ttu-id="414cf-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="414cf-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="414cf-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="414cf-114">invitedBy</span></span>      | <span data-ttu-id="414cf-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="414cf-115">[identitySet][]</span></span> | <span data-ttu-id="414cf-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="414cf-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="414cf-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="414cf-118">signInRequired</span></span> | <span data-ttu-id="414cf-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="414cf-119">Boolean</span></span>         | <span data-ttu-id="414cf-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="414cf-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="414cf-122">Заметки</span><span class="sxs-lookup"><span data-stu-id="414cf-122">Remarks</span></span>

<span data-ttu-id="414cf-123">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="414cf-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
