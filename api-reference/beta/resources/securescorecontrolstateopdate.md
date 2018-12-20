---
title: " Тип ресурса secureScoreControlStateUpdate"
description: Этот ресурс содержит журнал обновлен пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380968"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="80e90-103">Тип ресурса secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="80e90-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="80e90-104">Содержит журнал обновления пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).</span><span class="sxs-lookup"><span data-stu-id="80e90-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="80e90-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="80e90-105">Property</span></span> |<span data-ttu-id="80e90-106">Тип</span><span class="sxs-lookup"><span data-stu-id="80e90-106">Type</span></span> |<span data-ttu-id="80e90-107">Описание</span><span class="sxs-lookup"><span data-stu-id="80e90-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="80e90-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="80e90-108">assignedTo</span></span> | <span data-ttu-id="80e90-109">строка</span><span class="sxs-lookup"><span data-stu-id="80e90-109">string</span></span> | <span data-ttu-id="80e90-110">Назначение элемента управления для пользователя, который будет выполнять действия</span><span class="sxs-lookup"><span data-stu-id="80e90-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="80e90-111">comment</span><span class="sxs-lookup"><span data-stu-id="80e90-111">comment</span></span> | <span data-ttu-id="80e90-112">строка</span><span class="sxs-lookup"><span data-stu-id="80e90-112">string</span></span> | <span data-ttu-id="80e90-113">Предоставляет дополнительный комментарий об элементе управления</span><span class="sxs-lookup"><span data-stu-id="80e90-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="80e90-114">state</span><span class="sxs-lookup"><span data-stu-id="80e90-114">state</span></span> | <span data-ttu-id="80e90-115">строка</span><span class="sxs-lookup"><span data-stu-id="80e90-115">string</span></span> | <span data-ttu-id="80e90-116">Состояние элемента управления можно изменить с помощью команды ИСПРАВЛЕНИЯ (Ex: игнорируется, сторонних и т.д.)</span><span class="sxs-lookup"><span data-stu-id="80e90-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="80e90-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="80e90-117">updatedBy</span></span> | <span data-ttu-id="80e90-118">строка</span><span class="sxs-lookup"><span data-stu-id="80e90-118">string</span></span> |<span data-ttu-id="80e90-119">Идентификатор пользователя, который обновить состояние клиента</span><span class="sxs-lookup"><span data-stu-id="80e90-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="80e90-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="80e90-120">updatedDateTime</span></span> | <span data-ttu-id="80e90-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="80e90-121">DateTimeOffset?</span></span> |<span data-ttu-id="80e90-122">Время, в какой элемент управления обновить состояние</span><span class="sxs-lookup"><span data-stu-id="80e90-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="80e90-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80e90-123">JSON representation</span></span>
 <span data-ttu-id="80e90-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80e90-124">The following is a JSON representation of the resource.</span></span>
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
