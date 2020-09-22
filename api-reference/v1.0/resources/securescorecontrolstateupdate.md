---
title: Тип ресурса Секурескореконтролстатеупдате
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8f57c501ed2a4a47dbba163270feca8917fcce27
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984035"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="2e66d-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="2e66d-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="2e66d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e66d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e66d-105">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="2e66d-105">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="2e66d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e66d-106">Properties</span></span>

|<span data-ttu-id="2e66d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e66d-107">Property</span></span> |<span data-ttu-id="2e66d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2e66d-108">Type</span></span> |<span data-ttu-id="2e66d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e66d-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="2e66d-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="2e66d-110">assignedTo</span></span>|<span data-ttu-id="2e66d-111">String</span><span class="sxs-lookup"><span data-stu-id="2e66d-111">String</span></span>|<span data-ttu-id="2e66d-112">Назначает элемент управления пользователю, который будет выполнять действие.</span><span class="sxs-lookup"><span data-stu-id="2e66d-112">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="2e66d-113">comment</span><span class="sxs-lookup"><span data-stu-id="2e66d-113">comment</span></span>|<span data-ttu-id="2e66d-114">String</span><span class="sxs-lookup"><span data-stu-id="2e66d-114">String</span></span>|<span data-ttu-id="2e66d-115">Предоставляет необязательный комментарий об элементе управления.</span><span class="sxs-lookup"><span data-stu-id="2e66d-115">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="2e66d-116">state</span><span class="sxs-lookup"><span data-stu-id="2e66d-116">state</span></span>|<span data-ttu-id="2e66d-117">String</span><span class="sxs-lookup"><span data-stu-id="2e66d-117">String</span></span>|<span data-ttu-id="2e66d-118">Состояние элемента управления, которое можно изменить с помощью команды PATCH (например, игнорируется, thirdParty).</span><span class="sxs-lookup"><span data-stu-id="2e66d-118">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="2e66d-119">упдатедби</span><span class="sxs-lookup"><span data-stu-id="2e66d-119">updatedBy</span></span>|<span data-ttu-id="2e66d-120">String</span><span class="sxs-lookup"><span data-stu-id="2e66d-120">String</span></span>|<span data-ttu-id="2e66d-121">Идентификатор пользователя, который обновил состояние клиента.</span><span class="sxs-lookup"><span data-stu-id="2e66d-121">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="2e66d-122">упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="2e66d-122">updatedDateTime</span></span>|<span data-ttu-id="2e66d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e66d-123">DateTimeOffset</span></span>|<span data-ttu-id="2e66d-124">Время обновления состояния элемента управления.</span><span class="sxs-lookup"><span data-stu-id="2e66d-124">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e66d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e66d-125">JSON representation</span></span>
 <span data-ttu-id="2e66d-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e66d-126">The following is a JSON representation of the resource.</span></span>
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

