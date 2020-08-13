---
author: JeremyKelley
description: Ресурс DriveRecipient представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия invite.
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 64c2341eff772a5d26f6d17a3e646b561f4a9d37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505485"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="2ffae-103">Ресурс DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="2ffae-103">DriveRecipient resource</span></span>

<span data-ttu-id="2ffae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ffae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ffae-105">Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="2ffae-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ffae-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ffae-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2ffae-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ffae-107">Properties</span></span>
<span data-ttu-id="2ffae-108">Ниже перечислены свойства ресурса получателя.</span><span class="sxs-lookup"><span data-stu-id="2ffae-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="2ffae-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2ffae-109">Property name</span></span> | <span data-ttu-id="2ffae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2ffae-110">Type</span></span>   | <span data-ttu-id="2ffae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ffae-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2ffae-112">email</span><span class="sxs-lookup"><span data-stu-id="2ffae-112">email</span></span>         | <span data-ttu-id="2ffae-113">String</span><span class="sxs-lookup"><span data-stu-id="2ffae-113">String</span></span> | <span data-ttu-id="2ffae-114">Электронный адрес получателя (если с получателем связан электронный адрес).</span><span class="sxs-lookup"><span data-stu-id="2ffae-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="2ffae-115">alias</span><span class="sxs-lookup"><span data-stu-id="2ffae-115">alias</span></span>         | <span data-ttu-id="2ffae-116">String</span><span class="sxs-lookup"><span data-stu-id="2ffae-116">String</span></span> | <span data-ttu-id="2ffae-117">Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности).</span><span class="sxs-lookup"><span data-stu-id="2ffae-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="2ffae-118">objectId</span><span class="sxs-lookup"><span data-stu-id="2ffae-118">objectId</span></span>      | <span data-ttu-id="2ffae-119">String</span><span class="sxs-lookup"><span data-stu-id="2ffae-119">String</span></span> | <span data-ttu-id="2ffae-120">Уникальный идентификатор получателя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2ffae-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="2ffae-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="2ffae-121">Remarks</span></span>

<span data-ttu-id="2ffae-p101">При добавлении разрешений с помощью действия [invite](../api/driveitem-invite.md) в объекте DriveRecipient могут быть указаны свойства **email**, **alias** и **objectId**. Достаточно указать только одно из этих значений.</span><span class="sxs-lookup"><span data-stu-id="2ffae-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

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
