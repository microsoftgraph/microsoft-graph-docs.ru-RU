---
author: JeremyKelley
description: Ресурс SharingInvitation группирует элементы данных, связанные с приглашением, в единую структуру.
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6bbe39603ed4daad9c354b1c14ed6a68b3638c6d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520655"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="f89ab-103">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="f89ab-103">SharingInvitation resource type</span></span>

<span data-ttu-id="f89ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f89ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f89ab-105">Ресурс **SharingInvitation** группирует элементы данных, связанные с приглашением, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="f89ab-105">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f89ab-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f89ab-106">JSON representation</span></span>

<span data-ttu-id="f89ab-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f89ab-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f89ab-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f89ab-108">Properties</span></span>

| <span data-ttu-id="f89ab-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f89ab-109">Property Name</span></span>  | <span data-ttu-id="f89ab-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f89ab-110">Type</span></span>                          | <span data-ttu-id="f89ab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f89ab-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f89ab-112">email</span><span class="sxs-lookup"><span data-stu-id="f89ab-112">email</span></span>          | <span data-ttu-id="f89ab-113">String</span><span class="sxs-lookup"><span data-stu-id="f89ab-113">String</span></span>                        | <span data-ttu-id="f89ab-p101">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f89ab-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="f89ab-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="f89ab-116">invitedBy</span></span>      | [<span data-ttu-id="f89ab-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="f89ab-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="f89ab-p102">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f89ab-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="f89ab-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="f89ab-120">signInRequired</span></span> | <span data-ttu-id="f89ab-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f89ab-121">Boolean</span></span>                       | <span data-ttu-id="f89ab-p103">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f89ab-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="f89ab-124">Заметки</span><span class="sxs-lookup"><span data-stu-id="f89ab-124">Remarks</span></span> 

<span data-ttu-id="f89ab-125">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f89ab-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
