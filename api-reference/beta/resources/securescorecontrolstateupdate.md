---
title: " Тип ресурса secureScoreControlStateUpdate"
description: Этот ресурс содержит журнал обновлен пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574392"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="f021e-103">Тип ресурса secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="f021e-103">secureScoreControlStateUpdate resource type</span></span>

> <span data-ttu-id="f021e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f021e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f021e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f021e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f021e-106">Содержит журнал обновления пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).</span><span class="sxs-lookup"><span data-stu-id="f021e-106">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="f021e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f021e-107">Property</span></span>         | <span data-ttu-id="f021e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f021e-108">Type</span></span>           |<span data-ttu-id="f021e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f021e-109">Description</span></span>                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| <span data-ttu-id="f021e-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="f021e-110">assignedTo</span></span>      | <span data-ttu-id="f021e-111">string</span><span class="sxs-lookup"><span data-stu-id="f021e-111">string</span></span>         | <span data-ttu-id="f021e-112">Назначение элемента управления для пользователя, который будет выполнять действия</span><span class="sxs-lookup"><span data-stu-id="f021e-112">Assign the control to the user who will take the action</span></span>     |
| <span data-ttu-id="f021e-113">comment</span><span class="sxs-lookup"><span data-stu-id="f021e-113">comment</span></span>         | <span data-ttu-id="f021e-114">строка</span><span class="sxs-lookup"><span data-stu-id="f021e-114">string</span></span>         | <span data-ttu-id="f021e-115">Предоставляет дополнительный комментарий об элементе управления</span><span class="sxs-lookup"><span data-stu-id="f021e-115">Provides optional comment about the control</span></span>                 |
| <span data-ttu-id="f021e-116">state</span><span class="sxs-lookup"><span data-stu-id="f021e-116">state</span></span>           | <span data-ttu-id="f021e-117">string</span><span class="sxs-lookup"><span data-stu-id="f021e-117">string</span></span>         | <span data-ttu-id="f021e-118">Состояние элемента управления можно изменить с помощью команды ИСПРАВЛЕНИЯ (Ex: игнорируется, сторонних и т.д.)</span><span class="sxs-lookup"><span data-stu-id="f021e-118">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
| <span data-ttu-id="f021e-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="f021e-119">updatedBy</span></span>       | <span data-ttu-id="f021e-120">string</span><span class="sxs-lookup"><span data-stu-id="f021e-120">string</span></span>         |<span data-ttu-id="f021e-121">Идентификатор пользователя, который обновить состояние клиента</span><span class="sxs-lookup"><span data-stu-id="f021e-121">ID of the user who updated tenant state</span></span>                      |
| <span data-ttu-id="f021e-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f021e-122">updatedDateTime</span></span> | <span data-ttu-id="f021e-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f021e-123">DateTimeOffset</span></span> |<span data-ttu-id="f021e-124">Время, в какой элемент управления обновить состояние</span><span class="sxs-lookup"><span data-stu-id="f021e-124">Time at which control state was updated</span></span>                      |
 

## <a name="json-representation"></a><span data-ttu-id="f021e-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f021e-125">JSON representation</span></span>
 <span data-ttu-id="f021e-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f021e-126">The following is a JSON representation of the resource.</span></span>

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
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
