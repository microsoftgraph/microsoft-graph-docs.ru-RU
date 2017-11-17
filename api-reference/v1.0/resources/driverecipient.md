---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
ms.openlocfilehash: 53f6a5559cb90142a88b839a996cb2eedfd1037a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="driverecipient-resource"></a><span data-ttu-id="aff63-102">Ресурс DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="aff63-102">DriveRecipient resource type</span></span>

<span data-ttu-id="aff63-103">Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem_invite.md).</span><span class="sxs-lookup"><span data-stu-id="aff63-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem_invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aff63-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aff63-104">JSON representation</span></span>

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a><span data-ttu-id="aff63-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aff63-105">Properties</span></span>
<span data-ttu-id="aff63-106">Ниже перечислены свойства ресурса получателя.</span><span class="sxs-lookup"><span data-stu-id="aff63-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="aff63-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="aff63-107">Property name</span></span> | <span data-ttu-id="aff63-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aff63-108">Type</span></span>   | <span data-ttu-id="aff63-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aff63-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aff63-110">email</span><span class="sxs-lookup"><span data-stu-id="aff63-110">email</span></span>         | <span data-ttu-id="aff63-111">String</span><span class="sxs-lookup"><span data-stu-id="aff63-111">String</span></span> | <span data-ttu-id="aff63-112">Электронный адрес получателя (если с получателем связан электронный адрес).</span><span class="sxs-lookup"><span data-stu-id="aff63-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="aff63-113">alias</span><span class="sxs-lookup"><span data-stu-id="aff63-113">alias</span></span>         | <span data-ttu-id="aff63-114">String</span><span class="sxs-lookup"><span data-stu-id="aff63-114">String</span></span> | <span data-ttu-id="aff63-115">Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности).</span><span class="sxs-lookup"><span data-stu-id="aff63-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="aff63-116">objectId</span><span class="sxs-lookup"><span data-stu-id="aff63-116">objectId</span></span>      | <span data-ttu-id="aff63-117">String</span><span class="sxs-lookup"><span data-stu-id="aff63-117">String</span></span> | <span data-ttu-id="aff63-118">Уникальный идентификатор получателя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="aff63-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="aff63-119">Заметки</span><span class="sxs-lookup"><span data-stu-id="aff63-119">Remarks</span></span>

<span data-ttu-id="aff63-120">При добавлении разрешений с помощью действия [invite](../api/driveitem_invite.md) ресурс DriveRecipient может указать свойства **email**, **alias** и **objectId**.</span><span class="sxs-lookup"><span data-stu-id="aff63-120">When using invite to add permissions, the DriveRecipient can specify email, alias, or objectId. Only one of these values is required.</span></span>
<span data-ttu-id="aff63-121">Достаточно указать только одно из этих значений.</span><span class="sxs-lookup"><span data-stu-id="aff63-121">Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
