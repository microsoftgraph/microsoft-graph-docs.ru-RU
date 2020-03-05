---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: Ресурс SharingInvitation группирует элементы данных, связанные с приглашением, в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5e1b5434f025c48f1eea08d31a00b4bc5fc9d39f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446879"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="63da5-103">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="63da5-103">SharingInvitation resource type</span></span>

<span data-ttu-id="63da5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="63da5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63da5-105">Ресурс **SharingInvitation** группирует элементы данных, связанные с приглашением, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="63da5-105">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63da5-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63da5-106">JSON representation</span></span>

<span data-ttu-id="63da5-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63da5-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="63da5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="63da5-108">Properties</span></span>

| <span data-ttu-id="63da5-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="63da5-109">Property Name</span></span>  | <span data-ttu-id="63da5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="63da5-110">Type</span></span>            | <span data-ttu-id="63da5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="63da5-111">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="63da5-112">email</span><span class="sxs-lookup"><span data-stu-id="63da5-112">email</span></span>          | <span data-ttu-id="63da5-113">String</span><span class="sxs-lookup"><span data-stu-id="63da5-113">String</span></span>          | <span data-ttu-id="63da5-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="63da5-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="63da5-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="63da5-116">invitedBy</span></span>      | <span data-ttu-id="63da5-117">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="63da5-117">[identitySet][]</span></span> | <span data-ttu-id="63da5-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="63da5-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="63da5-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="63da5-120">signInRequired</span></span> | <span data-ttu-id="63da5-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="63da5-121">Boolean</span></span>         | <span data-ttu-id="63da5-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="63da5-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="63da5-124">Заметки</span><span class="sxs-lookup"><span data-stu-id="63da5-124">Remarks</span></span>

<span data-ttu-id="63da5-125">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="63da5-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
