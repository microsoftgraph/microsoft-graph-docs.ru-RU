---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f3b69838a6de68938efac12acdfbcd4fd977c684
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810407"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="90c90-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="90c90-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="90c90-104">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="90c90-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="90c90-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="90c90-105">Property</span></span> |<span data-ttu-id="90c90-106">Тип</span><span class="sxs-lookup"><span data-stu-id="90c90-106">Type</span></span> |<span data-ttu-id="90c90-107">Описание</span><span class="sxs-lookup"><span data-stu-id="90c90-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="90c90-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="90c90-108">assignedTo</span></span> | <span data-ttu-id="90c90-109">string</span><span class="sxs-lookup"><span data-stu-id="90c90-109">string</span></span> | <span data-ttu-id="90c90-110">Назначение элемента управления пользователю, который будет выполнять действие</span><span class="sxs-lookup"><span data-stu-id="90c90-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="90c90-111">comment</span><span class="sxs-lookup"><span data-stu-id="90c90-111">comment</span></span> | <span data-ttu-id="90c90-112">string</span><span class="sxs-lookup"><span data-stu-id="90c90-112">string</span></span> | <span data-ttu-id="90c90-113">Предоставляет необязательный комментарий об элементе управления</span><span class="sxs-lookup"><span data-stu-id="90c90-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="90c90-114">состояние</span><span class="sxs-lookup"><span data-stu-id="90c90-114">state</span></span> | <span data-ttu-id="90c90-115">string</span><span class="sxs-lookup"><span data-stu-id="90c90-115">string</span></span> | <span data-ttu-id="90c90-116">Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.)</span><span class="sxs-lookup"><span data-stu-id="90c90-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="90c90-117">упдатедби</span><span class="sxs-lookup"><span data-stu-id="90c90-117">updatedBy</span></span> | <span data-ttu-id="90c90-118">string</span><span class="sxs-lookup"><span data-stu-id="90c90-118">string</span></span> |<span data-ttu-id="90c90-119">Идентификатор пользователя, который обновил состояние клиента</span><span class="sxs-lookup"><span data-stu-id="90c90-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="90c90-120">упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="90c90-120">updatedDateTime</span></span> | <span data-ttu-id="90c90-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c90-121">DateTimeOffset</span></span> |<span data-ttu-id="90c90-122">Время обновления состояния элемента управления</span><span class="sxs-lookup"><span data-stu-id="90c90-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="90c90-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="90c90-123">JSON representation</span></span>
 <span data-ttu-id="90c90-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90c90-124">The following is a JSON representation of the resource.</span></span>
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
