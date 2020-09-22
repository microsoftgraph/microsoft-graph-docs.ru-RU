---
author: JeremyKelley
description: Ресурс DriveRecipient представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия invite.
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f703aa1bc9d12ec8b67aab0d80d641964b7b6096
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058475"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="2c4af-103">Ресурс DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="2c4af-103">DriveRecipient resource</span></span>

<span data-ttu-id="2c4af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c4af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c4af-105">Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="2c4af-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c4af-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c4af-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2c4af-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c4af-107">Properties</span></span>
<span data-ttu-id="2c4af-108">Ниже перечислены свойства ресурса получателя.</span><span class="sxs-lookup"><span data-stu-id="2c4af-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="2c4af-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2c4af-109">Property name</span></span> | <span data-ttu-id="2c4af-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2c4af-110">Type</span></span>   | <span data-ttu-id="2c4af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c4af-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2c4af-112">email</span><span class="sxs-lookup"><span data-stu-id="2c4af-112">email</span></span>         | <span data-ttu-id="2c4af-113">String</span><span class="sxs-lookup"><span data-stu-id="2c4af-113">String</span></span> | <span data-ttu-id="2c4af-114">Электронный адрес получателя (если с получателем связан электронный адрес).</span><span class="sxs-lookup"><span data-stu-id="2c4af-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="2c4af-115">alias</span><span class="sxs-lookup"><span data-stu-id="2c4af-115">alias</span></span>         | <span data-ttu-id="2c4af-116">String</span><span class="sxs-lookup"><span data-stu-id="2c4af-116">String</span></span> | <span data-ttu-id="2c4af-117">Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности).</span><span class="sxs-lookup"><span data-stu-id="2c4af-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="2c4af-118">objectId</span><span class="sxs-lookup"><span data-stu-id="2c4af-118">objectId</span></span>      | <span data-ttu-id="2c4af-119">String</span><span class="sxs-lookup"><span data-stu-id="2c4af-119">String</span></span> | <span data-ttu-id="2c4af-120">Уникальный идентификатор получателя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2c4af-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="2c4af-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="2c4af-121">Remarks</span></span>

<span data-ttu-id="2c4af-p101">При добавлении разрешений с помощью действия [invite](../api/driveitem-invite.md) в объекте DriveRecipient могут быть указаны свойства **email**, **alias** и **objectId**. Достаточно указать только одно из этих значений.</span><span class="sxs-lookup"><span data-stu-id="2c4af-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

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


