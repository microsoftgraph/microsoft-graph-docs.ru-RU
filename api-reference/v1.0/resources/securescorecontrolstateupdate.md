---
title: Тип ресурса Секурескореконтролстатеупдате
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0fe88741da75718b1509fd4f8015a37fcf7828bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446963"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="feb2a-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="feb2a-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="feb2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="feb2a-105">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="feb2a-105">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="feb2a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="feb2a-106">Properties</span></span>

|<span data-ttu-id="feb2a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="feb2a-107">Property</span></span> |<span data-ttu-id="feb2a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="feb2a-108">Type</span></span> |<span data-ttu-id="feb2a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="feb2a-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="feb2a-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="feb2a-110">assignedTo</span></span>|<span data-ttu-id="feb2a-111">String</span><span class="sxs-lookup"><span data-stu-id="feb2a-111">String</span></span>|<span data-ttu-id="feb2a-112">Назначает элемент управления пользователю, который будет выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="feb2a-112">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="feb2a-113">comment</span><span class="sxs-lookup"><span data-stu-id="feb2a-113">comment</span></span>|<span data-ttu-id="feb2a-114">String</span><span class="sxs-lookup"><span data-stu-id="feb2a-114">String</span></span>|<span data-ttu-id="feb2a-115">Предоставляет необязательный комментарий об элементе управления.</span><span class="sxs-lookup"><span data-stu-id="feb2a-115">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="feb2a-116">state</span><span class="sxs-lookup"><span data-stu-id="feb2a-116">state</span></span>|<span data-ttu-id="feb2a-117">String</span><span class="sxs-lookup"><span data-stu-id="feb2a-117">String</span></span>|<span data-ttu-id="feb2a-118">Состояние элемента управления, которое можно изменить с помощью команды PATCH (например, игнорируется, thirdParty).</span><span class="sxs-lookup"><span data-stu-id="feb2a-118">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="feb2a-119">упдатедби</span><span class="sxs-lookup"><span data-stu-id="feb2a-119">updatedBy</span></span>|<span data-ttu-id="feb2a-120">String</span><span class="sxs-lookup"><span data-stu-id="feb2a-120">String</span></span>|<span data-ttu-id="feb2a-121">Идентификатор пользователя, который обновил состояние клиента.</span><span class="sxs-lookup"><span data-stu-id="feb2a-121">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="feb2a-122">упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="feb2a-122">updatedDateTime</span></span>|<span data-ttu-id="feb2a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feb2a-123">DateTimeOffset</span></span>|<span data-ttu-id="feb2a-124">Время обновления состояния элемента управления.</span><span class="sxs-lookup"><span data-stu-id="feb2a-124">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="feb2a-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feb2a-125">JSON representation</span></span>
 <span data-ttu-id="feb2a-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feb2a-126">The following is a JSON representation of the resource.</span></span>
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
