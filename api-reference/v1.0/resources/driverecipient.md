---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4792a943598911cc2f0b8329016469ca157bda58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562722"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="42cc5-102">Ресурс DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="42cc5-102">DriveRecipient resource</span></span>

<span data-ttu-id="42cc5-103">Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="42cc5-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42cc5-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42cc5-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="42cc5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="42cc5-105">Properties</span></span>
<span data-ttu-id="42cc5-106">Ниже перечислены свойства ресурса получателя.</span><span class="sxs-lookup"><span data-stu-id="42cc5-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="42cc5-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="42cc5-107">Property name</span></span> | <span data-ttu-id="42cc5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="42cc5-108">Type</span></span>   | <span data-ttu-id="42cc5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="42cc5-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="42cc5-110">email</span><span class="sxs-lookup"><span data-stu-id="42cc5-110">email</span></span>         | <span data-ttu-id="42cc5-111">String</span><span class="sxs-lookup"><span data-stu-id="42cc5-111">String</span></span> | <span data-ttu-id="42cc5-112">Электронный адрес получателя (если с получателем связан электронный адрес).</span><span class="sxs-lookup"><span data-stu-id="42cc5-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="42cc5-113">alias</span><span class="sxs-lookup"><span data-stu-id="42cc5-113">alias</span></span>         | <span data-ttu-id="42cc5-114">String</span><span class="sxs-lookup"><span data-stu-id="42cc5-114">String</span></span> | <span data-ttu-id="42cc5-115">Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности).</span><span class="sxs-lookup"><span data-stu-id="42cc5-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="42cc5-116">objectId</span><span class="sxs-lookup"><span data-stu-id="42cc5-116">objectId</span></span>      | <span data-ttu-id="42cc5-117">String</span><span class="sxs-lookup"><span data-stu-id="42cc5-117">String</span></span> | <span data-ttu-id="42cc5-118">Уникальный идентификатор получателя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="42cc5-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="42cc5-119">Заметки</span><span class="sxs-lookup"><span data-stu-id="42cc5-119">Remarks</span></span>

<span data-ttu-id="42cc5-p101">При добавлении разрешений с помощью действия [invite](../api/driveitem-invite.md) в объекте DriveRecipient могут быть указаны свойства **email**, **alias** и **objectId**. Достаточно указать только одно из этих значений.</span><span class="sxs-lookup"><span data-stu-id="42cc5-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
