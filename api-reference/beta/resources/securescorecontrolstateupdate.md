---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92616569a87a6ccf91c17ea7c845b8185bd33e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965231"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="51b05-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="51b05-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="51b05-104">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="51b05-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="51b05-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="51b05-105">Property</span></span> |<span data-ttu-id="51b05-106">Тип</span><span class="sxs-lookup"><span data-stu-id="51b05-106">Type</span></span> |<span data-ttu-id="51b05-107">Описание</span><span class="sxs-lookup"><span data-stu-id="51b05-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="51b05-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="51b05-108">assignedTo</span></span> | <span data-ttu-id="51b05-109">string</span><span class="sxs-lookup"><span data-stu-id="51b05-109">string</span></span> | <span data-ttu-id="51b05-110">Назначение элемента управления пользователю, который будет выполнять действие</span><span class="sxs-lookup"><span data-stu-id="51b05-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="51b05-111">comment</span><span class="sxs-lookup"><span data-stu-id="51b05-111">comment</span></span> | <span data-ttu-id="51b05-112">строка</span><span class="sxs-lookup"><span data-stu-id="51b05-112">string</span></span> | <span data-ttu-id="51b05-113">Предоставляет необязательный комментарий об элементе управления</span><span class="sxs-lookup"><span data-stu-id="51b05-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="51b05-114">состояние</span><span class="sxs-lookup"><span data-stu-id="51b05-114">state</span></span> | <span data-ttu-id="51b05-115">string</span><span class="sxs-lookup"><span data-stu-id="51b05-115">string</span></span> | <span data-ttu-id="51b05-116">Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.)</span><span class="sxs-lookup"><span data-stu-id="51b05-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="51b05-117">Упдатедби</span><span class="sxs-lookup"><span data-stu-id="51b05-117">updatedBy</span></span> | <span data-ttu-id="51b05-118">string</span><span class="sxs-lookup"><span data-stu-id="51b05-118">string</span></span> |<span data-ttu-id="51b05-119">Идентификатор пользователя, который обновил состояние клиента</span><span class="sxs-lookup"><span data-stu-id="51b05-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="51b05-120">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="51b05-120">updatedDateTime</span></span> | <span data-ttu-id="51b05-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51b05-121">DateTimeOffset</span></span> |<span data-ttu-id="51b05-122">Время обновления состояния элемента управления</span><span class="sxs-lookup"><span data-stu-id="51b05-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="51b05-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51b05-123">JSON representation</span></span>
 <span data-ttu-id="51b05-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51b05-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
