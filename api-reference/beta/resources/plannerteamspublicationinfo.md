---
title: Тип ресурса plannerTeamsPublicationInfo
description: Содержит подробные сведения о процессе публикации, который создал plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9db73bb5a914a848f3e19e079321681b22510e8e
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883259"
---
# <a name="plannerteamspublicationinfo-resource-type"></a><span data-ttu-id="87845-103">Тип ресурса plannerTeamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="87845-103">plannerTeamsPublicationInfo resource type</span></span>

<span data-ttu-id="87845-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87845-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87845-105">Содержит подробные сведения о процессе публикации, который создал [plannerTask.](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="87845-105">Contains detailed information about the publication process that created a [plannerTask](plannertask.md).</span></span> <span data-ttu-id="87845-106">Процесс публикации создает копии задач на основе шаблона.</span><span class="sxs-lookup"><span data-stu-id="87845-106">A publication process creates copies of tasks based on a template.</span></span> <span data-ttu-id="87845-107">Эти задачи создаются в нескольких планах и имеют ограниченные разрешения для пользователей; Например, их нельзя удалить, а пользователям может быть заблокировано редактирование определенных полей.</span><span class="sxs-lookup"><span data-stu-id="87845-107">These tasks are created in multiple plans, and have restricted permissions for the users; for example, they cannot be deleted and users might be blocked from editing certain fields.</span></span> <span data-ttu-id="87845-108">Публикация используется для распространения задач по всей организации и централизованного отслеживания их хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="87845-108">Publication is used to distribute tasks across an organization and track their progress centrally.</span></span>

## <a name="properties"></a><span data-ttu-id="87845-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="87845-109">Properties</span></span>
|<span data-ttu-id="87845-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="87845-110">Property</span></span>|<span data-ttu-id="87845-111">Тип</span><span class="sxs-lookup"><span data-stu-id="87845-111">Type</span></span>|<span data-ttu-id="87845-112">Описание</span><span class="sxs-lookup"><span data-stu-id="87845-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87845-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87845-113">lastModifiedDateTime</span></span>|<span data-ttu-id="87845-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87845-114">DateTimeOffset</span></span>|<span data-ttu-id="87845-115">Дата и время последнего изменения этой задачи в процессе публикации.</span><span class="sxs-lookup"><span data-stu-id="87845-115">The date and time when this task was last modified by the publication process.</span></span> <span data-ttu-id="87845-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87845-116">Read-only.</span></span> |
|<span data-ttu-id="87845-117">publicationId</span><span class="sxs-lookup"><span data-stu-id="87845-117">publicationId</span></span>|<span data-ttu-id="87845-118">Строка</span><span class="sxs-lookup"><span data-stu-id="87845-118">String</span></span>| <span data-ttu-id="87845-119">Идентификатор публикации.</span><span class="sxs-lookup"><span data-stu-id="87845-119">The identifier of the publication.</span></span> <span data-ttu-id="87845-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87845-120">Read-only.</span></span>|
|<span data-ttu-id="87845-121">publishedToPlanId</span><span class="sxs-lookup"><span data-stu-id="87845-121">publishedToPlanId</span></span>|<span data-ttu-id="87845-122">Строка</span><span class="sxs-lookup"><span data-stu-id="87845-122">String</span></span>|<span data-ttu-id="87845-123">Идентификатор **планировщика,** в который изначально была помещена эта задача.</span><span class="sxs-lookup"><span data-stu-id="87845-123">The identifier of the **plannerPlan** this task was originally placed in.</span></span> <span data-ttu-id="87845-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87845-124">Read-only.</span></span> |
|<span data-ttu-id="87845-125">publishingTeamId</span><span class="sxs-lookup"><span data-stu-id="87845-125">publishingTeamId</span></span>|<span data-ttu-id="87845-126">Строка</span><span class="sxs-lookup"><span data-stu-id="87845-126">String</span></span>| <span data-ttu-id="87845-127">Идентификатор команды, [которая](team.md) инициировала процесс публикации.</span><span class="sxs-lookup"><span data-stu-id="87845-127">The identifier of the [team](team.md) that initiated the publication process.</span></span> <span data-ttu-id="87845-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87845-128">Read-only.</span></span>|
|<span data-ttu-id="87845-129">publishingTeamName</span><span class="sxs-lookup"><span data-stu-id="87845-129">publishingTeamName</span></span>|<span data-ttu-id="87845-130">Строка</span><span class="sxs-lookup"><span data-stu-id="87845-130">String</span></span>|<span data-ttu-id="87845-131">Отображаемое имя команды, которая инициировала процесс публикации.</span><span class="sxs-lookup"><span data-stu-id="87845-131">The display name of the team that initiated the publication process.</span></span> <span data-ttu-id="87845-132">Это отображаемого имени только для ссылки и может не представлять наиболее последние имена команды.</span><span class="sxs-lookup"><span data-stu-id="87845-132">This display name is for reference only, and might not represent the most up-to-date name of the team.</span></span> <span data-ttu-id="87845-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87845-133">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="87845-134">Связи</span><span class="sxs-lookup"><span data-stu-id="87845-134">Relationships</span></span>
<span data-ttu-id="87845-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="87845-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87845-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="87845-136">JSON representation</span></span>
<span data-ttu-id="87845-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87845-137">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTeamsPublicationInfo",
  "publicationId": "String",
  "publishingTeamId": "String",
  "publishingTeamName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishedToPlanId": "String"
}
```

