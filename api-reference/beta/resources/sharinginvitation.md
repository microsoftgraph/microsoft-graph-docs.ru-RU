---
author: JeremyKelley
description: Ресурс SharingInvitation группирует элементы данных, связанные с приглашением, в единую структуру.
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4c6a26e2acfdc4bca1eed34191ba78f333b5fc9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997706"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="6a2ba-103">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="6a2ba-103">SharingInvitation resource type</span></span>

<span data-ttu-id="6a2ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a2ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a2ba-105">Ресурс **SharingInvitation** группирует элементы данных, связанные с приглашением, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="6a2ba-105">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a2ba-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a2ba-106">JSON representation</span></span>

<span data-ttu-id="6a2ba-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6a2ba-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="6a2ba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a2ba-108">Properties</span></span>

| <span data-ttu-id="6a2ba-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6a2ba-109">Property Name</span></span>  | <span data-ttu-id="6a2ba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6a2ba-110">Type</span></span>                          | <span data-ttu-id="6a2ba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a2ba-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6a2ba-112">email</span><span class="sxs-lookup"><span data-stu-id="6a2ba-112">email</span></span>          | <span data-ttu-id="6a2ba-113">String</span><span class="sxs-lookup"><span data-stu-id="6a2ba-113">String</span></span>                        | <span data-ttu-id="6a2ba-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a2ba-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="6a2ba-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="6a2ba-116">invitedBy</span></span>      | [<span data-ttu-id="6a2ba-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="6a2ba-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="6a2ba-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a2ba-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="6a2ba-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="6a2ba-120">signInRequired</span></span> | <span data-ttu-id="6a2ba-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a2ba-121">Boolean</span></span>                       | <span data-ttu-id="6a2ba-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a2ba-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="6a2ba-124">Заметки</span><span class="sxs-lookup"><span data-stu-id="6a2ba-124">Remarks</span></span> 

<span data-ttu-id="6a2ba-125">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6a2ba-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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


