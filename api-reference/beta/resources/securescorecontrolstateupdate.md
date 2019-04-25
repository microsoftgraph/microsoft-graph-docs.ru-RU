---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549141"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="14a7f-103">Тип ресурса Секурескореконтролстатеупдате</span><span class="sxs-lookup"><span data-stu-id="14a7f-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="14a7f-104">Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).</span><span class="sxs-lookup"><span data-stu-id="14a7f-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="14a7f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="14a7f-105">Property</span></span> |<span data-ttu-id="14a7f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="14a7f-106">Type</span></span> |<span data-ttu-id="14a7f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="14a7f-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="14a7f-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="14a7f-108">assignedTo</span></span> | <span data-ttu-id="14a7f-109">string</span><span class="sxs-lookup"><span data-stu-id="14a7f-109">string</span></span> | <span data-ttu-id="14a7f-110">Назначение элемента управления пользователю, который будет выполнять действие</span><span class="sxs-lookup"><span data-stu-id="14a7f-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="14a7f-111">comment</span><span class="sxs-lookup"><span data-stu-id="14a7f-111">comment</span></span> | <span data-ttu-id="14a7f-112">строка</span><span class="sxs-lookup"><span data-stu-id="14a7f-112">string</span></span> | <span data-ttu-id="14a7f-113">Предоставляет необязательный комментарий об элементе управления</span><span class="sxs-lookup"><span data-stu-id="14a7f-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="14a7f-114">состояние</span><span class="sxs-lookup"><span data-stu-id="14a7f-114">state</span></span> | <span data-ttu-id="14a7f-115">string</span><span class="sxs-lookup"><span data-stu-id="14a7f-115">string</span></span> | <span data-ttu-id="14a7f-116">Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.)</span><span class="sxs-lookup"><span data-stu-id="14a7f-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="14a7f-117">Упдатедби</span><span class="sxs-lookup"><span data-stu-id="14a7f-117">updatedBy</span></span> | <span data-ttu-id="14a7f-118">string</span><span class="sxs-lookup"><span data-stu-id="14a7f-118">string</span></span> |<span data-ttu-id="14a7f-119">Идентификатор пользователя, который обновил состояние клиента</span><span class="sxs-lookup"><span data-stu-id="14a7f-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="14a7f-120">Упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="14a7f-120">updatedDateTime</span></span> | <span data-ttu-id="14a7f-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="14a7f-121">DateTimeOffset?</span></span> |<span data-ttu-id="14a7f-122">Время обновления состояния элемента управления</span><span class="sxs-lookup"><span data-stu-id="14a7f-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="14a7f-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14a7f-123">JSON representation</span></span>
 <span data-ttu-id="14a7f-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14a7f-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
