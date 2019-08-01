---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: Ресурс SharingInvitation группирует элементы данных, связанные с приглашением, в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 011402b40b601642a048b91e3b3f66de0792aaf2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034246"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="ec79e-103">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="ec79e-103">SharingInvitation resource type</span></span>

<span data-ttu-id="ec79e-104">Ресурс **SharingInvitation** группирует элементы данных, связанные с приглашением, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="ec79e-104">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec79e-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec79e-105">JSON representation</span></span>

<span data-ttu-id="ec79e-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec79e-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ec79e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec79e-107">Properties</span></span>

| <span data-ttu-id="ec79e-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ec79e-108">Property Name</span></span>  | <span data-ttu-id="ec79e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ec79e-109">Type</span></span>            | <span data-ttu-id="ec79e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ec79e-110">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="ec79e-111">email</span><span class="sxs-lookup"><span data-stu-id="ec79e-111">email</span></span>          | <span data-ttu-id="ec79e-112">String</span><span class="sxs-lookup"><span data-stu-id="ec79e-112">String</span></span>          | <span data-ttu-id="ec79e-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec79e-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="ec79e-115">invitedBy</span><span class="sxs-lookup"><span data-stu-id="ec79e-115">invitedBy</span></span>      | <span data-ttu-id="ec79e-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ec79e-116">[identitySet][]</span></span> | <span data-ttu-id="ec79e-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec79e-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="ec79e-119">signInRequired</span><span class="sxs-lookup"><span data-stu-id="ec79e-119">signInRequired</span></span> | <span data-ttu-id="ec79e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec79e-120">Boolean</span></span>         | <span data-ttu-id="ec79e-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec79e-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="ec79e-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="ec79e-123">Remarks</span></span>

<span data-ttu-id="ec79e-124">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ec79e-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
