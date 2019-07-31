---
author: JeremyKelley
description: Ресурс DriveRecipient представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия invite.
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f86b79567b4148934f1c9624124026472fbb3395
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012711"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="8c5ea-103">Ресурс DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="8c5ea-103">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c5ea-104">Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="8c5ea-104">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c5ea-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c5ea-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8c5ea-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c5ea-106">Properties</span></span>
<span data-ttu-id="8c5ea-107">Ниже перечислены свойства ресурса получателя.</span><span class="sxs-lookup"><span data-stu-id="8c5ea-107">The recipients resource has these properties.</span></span>

| <span data-ttu-id="8c5ea-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8c5ea-108">Property name</span></span> | <span data-ttu-id="8c5ea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c5ea-109">Type</span></span>   | <span data-ttu-id="8c5ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c5ea-110">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8c5ea-111">email</span><span class="sxs-lookup"><span data-stu-id="8c5ea-111">email</span></span>         | <span data-ttu-id="8c5ea-112">String</span><span class="sxs-lookup"><span data-stu-id="8c5ea-112">String</span></span> | <span data-ttu-id="8c5ea-113">Электронный адрес получателя (если с получателем связан электронный адрес).</span><span class="sxs-lookup"><span data-stu-id="8c5ea-113">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="8c5ea-114">alias</span><span class="sxs-lookup"><span data-stu-id="8c5ea-114">alias</span></span>         | <span data-ttu-id="8c5ea-115">String</span><span class="sxs-lookup"><span data-stu-id="8c5ea-115">String</span></span> | <span data-ttu-id="8c5ea-116">Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности).</span><span class="sxs-lookup"><span data-stu-id="8c5ea-116">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="8c5ea-117">objectId</span><span class="sxs-lookup"><span data-stu-id="8c5ea-117">objectId</span></span>      | <span data-ttu-id="8c5ea-118">String</span><span class="sxs-lookup"><span data-stu-id="8c5ea-118">String</span></span> | <span data-ttu-id="8c5ea-119">Уникальный идентификатор получателя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="8c5ea-119">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="8c5ea-120">Заметки</span><span class="sxs-lookup"><span data-stu-id="8c5ea-120">Remarks</span></span>

<span data-ttu-id="8c5ea-p101">При добавлении разрешений с помощью действия [invite](../api/driveitem-invite.md) в объекте DriveRecipient могут быть указаны свойства **email**, **alias** и **objectId**. Достаточно указать только одно из этих значений.</span><span class="sxs-lookup"><span data-stu-id="8c5ea-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": []
}
-->
