---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: ba909158ce0ba28b6af20b8dbff858c65f07cbe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080858"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="74960-102">Тип ресурса SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="74960-102">SharingInvitation resource type</span></span>

> <span data-ttu-id="74960-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74960-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74960-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74960-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74960-105">Ресурс **SharingInvitation** — это единая структура, объединяющая элементы данных, связанные с приглашениями.</span><span class="sxs-lookup"><span data-stu-id="74960-105">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74960-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74960-106">JSON representation</span></span>

<span data-ttu-id="74960-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="74960-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="74960-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="74960-108">Properties</span></span>

| <span data-ttu-id="74960-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="74960-109">Property Name</span></span>  | <span data-ttu-id="74960-110">Тип</span><span class="sxs-lookup"><span data-stu-id="74960-110">Type</span></span>                          | <span data-ttu-id="74960-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74960-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="74960-112">email</span><span class="sxs-lookup"><span data-stu-id="74960-112">email</span></span>          | <span data-ttu-id="74960-113">String</span><span class="sxs-lookup"><span data-stu-id="74960-113">String</span></span>                        | <span data-ttu-id="74960-p102">Электронный адрес получателя приглашения к совместному использованию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74960-p102">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="74960-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="74960-116">invitedBy</span></span>      | [<span data-ttu-id="74960-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="74960-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="74960-p103">Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74960-p103">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="74960-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="74960-120">signInRequired</span></span> | <span data-ttu-id="74960-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="74960-121">Boolean</span></span>                       | <span data-ttu-id="74960-p104">Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74960-p104">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="74960-124">Заметки</span><span class="sxs-lookup"><span data-stu-id="74960-124">Remarks</span></span> 

<span data-ttu-id="74960-125">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="74960-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": ""
}-->
