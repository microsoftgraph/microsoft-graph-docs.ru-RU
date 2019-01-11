---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.openlocfilehash: f1bc78a8ec0648ce90221e4ad1f4473e49b625b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863730"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="bc98f-102">Ресурс DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="bc98f-102">DriveRecipient resource</span></span>

> <span data-ttu-id="bc98f-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc98f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc98f-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc98f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc98f-105">Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="bc98f-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc98f-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc98f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bc98f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc98f-107">Properties</span></span>
<span data-ttu-id="bc98f-108">Ниже перечислены свойства ресурса получателя.</span><span class="sxs-lookup"><span data-stu-id="bc98f-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="bc98f-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bc98f-109">Property name</span></span> | <span data-ttu-id="bc98f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bc98f-110">Type</span></span>   | <span data-ttu-id="bc98f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bc98f-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="bc98f-112">email</span><span class="sxs-lookup"><span data-stu-id="bc98f-112">email</span></span>         | <span data-ttu-id="bc98f-113">String</span><span class="sxs-lookup"><span data-stu-id="bc98f-113">String</span></span> | <span data-ttu-id="bc98f-114">Электронный адрес получателя (если с получателем связан электронный адрес).</span><span class="sxs-lookup"><span data-stu-id="bc98f-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="bc98f-115">alias</span><span class="sxs-lookup"><span data-stu-id="bc98f-115">alias</span></span>         | <span data-ttu-id="bc98f-116">String</span><span class="sxs-lookup"><span data-stu-id="bc98f-116">String</span></span> | <span data-ttu-id="bc98f-117">Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности).</span><span class="sxs-lookup"><span data-stu-id="bc98f-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="bc98f-118">objectId</span><span class="sxs-lookup"><span data-stu-id="bc98f-118">objectId</span></span>      | <span data-ttu-id="bc98f-119">String</span><span class="sxs-lookup"><span data-stu-id="bc98f-119">String</span></span> | <span data-ttu-id="bc98f-120">Уникальный идентификатор получателя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="bc98f-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="bc98f-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="bc98f-121">Remarks</span></span>

<span data-ttu-id="bc98f-p102">При добавлении разрешений с помощью действия [invite](../api/driveitem-invite.md) в объекте DriveRecipient могут быть указаны свойства **email**, **alias** и **objectId**. Достаточно указать только одно из этих значений.</span><span class="sxs-lookup"><span data-stu-id="bc98f-p102">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
