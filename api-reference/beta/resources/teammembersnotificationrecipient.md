---
title: тип ресурса teamMembersNotificationRecipient
description: Представляет получателя уведомления, отправленного в канале Microsoft Teams действий. Получатель состоит из членов группы.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a025b6c4ecb9c2eba9f6b31f5eedf108f6ed87ed
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211397"
---
# <a name="teammembersnotificationrecipient-resource-type"></a><span data-ttu-id="f4170-104">тип ресурса teamMembersNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="f4170-104">teamMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="f4170-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4170-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4170-106">Представляет получателя уведомления, отправленного в канале Microsoft Teams действий.</span><span class="sxs-lookup"><span data-stu-id="f4170-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="f4170-107">Получатель состоит из членов группы.</span><span class="sxs-lookup"><span data-stu-id="f4170-107">The recipient consists of the team members.</span></span>

<span data-ttu-id="f4170-108">Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="f4170-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f4170-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4170-109">Properties</span></span>
|<span data-ttu-id="f4170-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4170-110">Property</span></span>|<span data-ttu-id="f4170-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f4170-111">Type</span></span>|<span data-ttu-id="f4170-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f4170-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4170-113">teamId</span><span class="sxs-lookup"><span data-stu-id="f4170-113">teamId</span></span>|<span data-ttu-id="f4170-114">String</span><span class="sxs-lookup"><span data-stu-id="f4170-114">String</span></span>|<span data-ttu-id="f4170-115">Идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="f4170-115">The team's identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4170-116">Связи</span><span class="sxs-lookup"><span data-stu-id="f4170-116">Relationships</span></span>
<span data-ttu-id="f4170-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f4170-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4170-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f4170-118">JSON representation</span></span>
<span data-ttu-id="f4170-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4170-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.teamMembersNotificationRecipient",
  "teamId": "String"
}
```

