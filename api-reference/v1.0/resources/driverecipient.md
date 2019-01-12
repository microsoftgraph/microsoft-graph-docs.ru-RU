---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bd1b4466a361af031b9c8e11be63acb46044351a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983382"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="85a09-102">Ресурс DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="85a09-102">DriveRecipient resource</span></span>

<span data-ttu-id="85a09-103">Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="85a09-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85a09-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85a09-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="85a09-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="85a09-105">Properties</span></span>
<span data-ttu-id="85a09-106">Ниже перечислены свойства ресурса получателя.</span><span class="sxs-lookup"><span data-stu-id="85a09-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="85a09-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="85a09-107">Property name</span></span> | <span data-ttu-id="85a09-108">Тип</span><span class="sxs-lookup"><span data-stu-id="85a09-108">Type</span></span>   | <span data-ttu-id="85a09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="85a09-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="85a09-110">email</span><span class="sxs-lookup"><span data-stu-id="85a09-110">email</span></span>         | <span data-ttu-id="85a09-111">String</span><span class="sxs-lookup"><span data-stu-id="85a09-111">String</span></span> | <span data-ttu-id="85a09-112">Электронный адрес получателя (если с получателем связан электронный адрес).</span><span class="sxs-lookup"><span data-stu-id="85a09-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="85a09-113">alias</span><span class="sxs-lookup"><span data-stu-id="85a09-113">alias</span></span>         | <span data-ttu-id="85a09-114">String</span><span class="sxs-lookup"><span data-stu-id="85a09-114">String</span></span> | <span data-ttu-id="85a09-115">Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности).</span><span class="sxs-lookup"><span data-stu-id="85a09-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="85a09-116">objectId</span><span class="sxs-lookup"><span data-stu-id="85a09-116">objectId</span></span>      | <span data-ttu-id="85a09-117">String</span><span class="sxs-lookup"><span data-stu-id="85a09-117">String</span></span> | <span data-ttu-id="85a09-118">Уникальный идентификатор получателя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="85a09-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="85a09-119">Заметки</span><span class="sxs-lookup"><span data-stu-id="85a09-119">Remarks</span></span>

<span data-ttu-id="85a09-p101">При добавлении разрешений с помощью действия [invite](../api/driveitem-invite.md) в объекте DriveRecipient могут быть указаны свойства **email**, **alias** и **objectId**. Достаточно указать только одно из этих значений.</span><span class="sxs-lookup"><span data-stu-id="85a09-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
