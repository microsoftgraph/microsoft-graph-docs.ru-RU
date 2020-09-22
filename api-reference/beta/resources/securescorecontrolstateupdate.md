---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d1678d4fe77ade738f7eb298221772ced381e2d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087553"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="af601-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="af601-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="af601-104">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="af601-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="af601-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="af601-105">Property</span></span> |<span data-ttu-id="af601-106">Тип</span><span class="sxs-lookup"><span data-stu-id="af601-106">Type</span></span> |<span data-ttu-id="af601-107">Описание</span><span class="sxs-lookup"><span data-stu-id="af601-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="af601-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="af601-108">assignedTo</span></span> | <span data-ttu-id="af601-109">string</span><span class="sxs-lookup"><span data-stu-id="af601-109">string</span></span> | <span data-ttu-id="af601-110">Назначение элемента управления пользователю, который будет выполнять действие</span><span class="sxs-lookup"><span data-stu-id="af601-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="af601-111">comment</span><span class="sxs-lookup"><span data-stu-id="af601-111">comment</span></span> | <span data-ttu-id="af601-112">string</span><span class="sxs-lookup"><span data-stu-id="af601-112">string</span></span> | <span data-ttu-id="af601-113">Предоставляет необязательный комментарий об элементе управления</span><span class="sxs-lookup"><span data-stu-id="af601-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="af601-114">состояние</span><span class="sxs-lookup"><span data-stu-id="af601-114">state</span></span> | <span data-ttu-id="af601-115">string</span><span class="sxs-lookup"><span data-stu-id="af601-115">string</span></span> | <span data-ttu-id="af601-116">Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.)</span><span class="sxs-lookup"><span data-stu-id="af601-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="af601-117">упдатедби</span><span class="sxs-lookup"><span data-stu-id="af601-117">updatedBy</span></span> | <span data-ttu-id="af601-118">string</span><span class="sxs-lookup"><span data-stu-id="af601-118">string</span></span> |<span data-ttu-id="af601-119">Идентификатор пользователя, который обновил состояние клиента</span><span class="sxs-lookup"><span data-stu-id="af601-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="af601-120">упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="af601-120">updatedDateTime</span></span> | <span data-ttu-id="af601-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af601-121">DateTimeOffset</span></span> |<span data-ttu-id="af601-122">Время обновления состояния элемента управления</span><span class="sxs-lookup"><span data-stu-id="af601-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="af601-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="af601-123">JSON representation</span></span>
 <span data-ttu-id="af601-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af601-124">The following is a JSON representation of the resource.</span></span>
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


