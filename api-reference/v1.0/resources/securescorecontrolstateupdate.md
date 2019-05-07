---
title: Тип ресурса Секурескореконтролстатеупдате
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
author: preetikr
ms.openlocfilehash: ac66fb2085949e375c79b18bfdfd39e84392159d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629252"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="69c98-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="69c98-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="69c98-104">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="69c98-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="69c98-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="69c98-105">Properties</span></span>

|<span data-ttu-id="69c98-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="69c98-106">Property</span></span> |<span data-ttu-id="69c98-107">Тип</span><span class="sxs-lookup"><span data-stu-id="69c98-107">Type</span></span> |<span data-ttu-id="69c98-108">Описание</span><span class="sxs-lookup"><span data-stu-id="69c98-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="69c98-109">assignedTo</span><span class="sxs-lookup"><span data-stu-id="69c98-109">assignedTo</span></span>|<span data-ttu-id="69c98-110">String</span><span class="sxs-lookup"><span data-stu-id="69c98-110">String</span></span>|<span data-ttu-id="69c98-111">Назначает элемент управления пользователю, который будет выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="69c98-111">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="69c98-112">comment</span><span class="sxs-lookup"><span data-stu-id="69c98-112">comment</span></span>|<span data-ttu-id="69c98-113">String</span><span class="sxs-lookup"><span data-stu-id="69c98-113">String</span></span>|<span data-ttu-id="69c98-114">Предоставляет необязательный комментарий об элементе управления.</span><span class="sxs-lookup"><span data-stu-id="69c98-114">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="69c98-115">state</span><span class="sxs-lookup"><span data-stu-id="69c98-115">state</span></span>|<span data-ttu-id="69c98-116">String</span><span class="sxs-lookup"><span data-stu-id="69c98-116">String</span></span>|<span data-ttu-id="69c98-117">Состояние элемента управления, которое можно изменить с помощью команды PATCH (например, игнорируется, thirdParty).</span><span class="sxs-lookup"><span data-stu-id="69c98-117">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="69c98-118">Упдатедби</span><span class="sxs-lookup"><span data-stu-id="69c98-118">updatedBy</span></span>|<span data-ttu-id="69c98-119">String</span><span class="sxs-lookup"><span data-stu-id="69c98-119">String</span></span>|<span data-ttu-id="69c98-120">Идентификатор пользователя, который обновил состояние клиента.</span><span class="sxs-lookup"><span data-stu-id="69c98-120">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="69c98-121">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="69c98-121">updatedDateTime</span></span>|<span data-ttu-id="69c98-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69c98-122">DateTimeOffset</span></span>|<span data-ttu-id="69c98-123">Время обновления состояния элемента управления.</span><span class="sxs-lookup"><span data-stu-id="69c98-123">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="69c98-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="69c98-124">JSON representation</span></span>
 <span data-ttu-id="69c98-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69c98-125">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
    
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
