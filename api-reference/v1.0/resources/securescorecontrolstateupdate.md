---
title: Тип ресурса Секурескореконтролстатеупдате
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e051f2c4319a2b2ae1e3dbd9ba633785a345c4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034477"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="a7d0e-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="a7d0e-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="a7d0e-104">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="a7d0e-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="a7d0e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7d0e-105">Properties</span></span>

|<span data-ttu-id="a7d0e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7d0e-106">Property</span></span> |<span data-ttu-id="a7d0e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a7d0e-107">Type</span></span> |<span data-ttu-id="a7d0e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d0e-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="a7d0e-109">assignedTo</span><span class="sxs-lookup"><span data-stu-id="a7d0e-109">assignedTo</span></span>|<span data-ttu-id="a7d0e-110">String</span><span class="sxs-lookup"><span data-stu-id="a7d0e-110">String</span></span>|<span data-ttu-id="a7d0e-111">Назначает элемент управления пользователю, который будет выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="a7d0e-111">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="a7d0e-112">comment</span><span class="sxs-lookup"><span data-stu-id="a7d0e-112">comment</span></span>|<span data-ttu-id="a7d0e-113">String</span><span class="sxs-lookup"><span data-stu-id="a7d0e-113">String</span></span>|<span data-ttu-id="a7d0e-114">Предоставляет необязательный комментарий об элементе управления.</span><span class="sxs-lookup"><span data-stu-id="a7d0e-114">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="a7d0e-115">state</span><span class="sxs-lookup"><span data-stu-id="a7d0e-115">state</span></span>|<span data-ttu-id="a7d0e-116">String</span><span class="sxs-lookup"><span data-stu-id="a7d0e-116">String</span></span>|<span data-ttu-id="a7d0e-117">Состояние элемента управления, которое можно изменить с помощью команды PATCH (например, игнорируется, thirdParty).</span><span class="sxs-lookup"><span data-stu-id="a7d0e-117">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="a7d0e-118">Упдатедби</span><span class="sxs-lookup"><span data-stu-id="a7d0e-118">updatedBy</span></span>|<span data-ttu-id="a7d0e-119">String</span><span class="sxs-lookup"><span data-stu-id="a7d0e-119">String</span></span>|<span data-ttu-id="a7d0e-120">Идентификатор пользователя, который обновил состояние клиента.</span><span class="sxs-lookup"><span data-stu-id="a7d0e-120">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="a7d0e-121">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a7d0e-121">updatedDateTime</span></span>|<span data-ttu-id="a7d0e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7d0e-122">DateTimeOffset</span></span>|<span data-ttu-id="a7d0e-123">Время обновления состояния элемента управления.</span><span class="sxs-lookup"><span data-stu-id="a7d0e-123">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a7d0e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7d0e-124">JSON representation</span></span>
 <span data-ttu-id="a7d0e-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7d0e-125">The following is a JSON representation of the resource.</span></span>
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
