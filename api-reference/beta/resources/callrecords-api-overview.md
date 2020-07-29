---
title: Работа с API записей звонков в Microsoft Graph
description: API записей звонков Microsoft Graph позволяет извлекать данные об использовании и диагностике для звонков и собраний по сети в вашей организации.
author: stephenjust
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 3fae40563bbd89b5792d75b5d8a0a51c1cda17e3
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509884"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a><span data-ttu-id="1f275-103">Работа с API записей звонков в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1f275-103">Working with the call records API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f275-104">Записи звонков содержат сведения об использовании и диагностике, касающиеся звонков и собраний по сети в вашей организации при применении Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1f275-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="1f275-105">Вы можете использовать API записей звонков, чтобы подписаться на записи звонков и искать их по идентификаторам.</span><span class="sxs-lookup"><span data-stu-id="1f275-105">You can use the call records APIs to subscribe to call records and look up call records by IDs.</span></span>

<span data-ttu-id="1f275-106">API записи звонков задается в подпространстве имен OData, `microsoft.graph.callRecords`.</span><span class="sxs-lookup"><span data-stu-id="1f275-106">The call records API is defined in the OData sub-namespace, `microsoft.graph.callRecords`.</span></span>

## <a name="key-resource-types"></a><span data-ttu-id="1f275-107">Ключевые типы ресурсов</span><span class="sxs-lookup"><span data-stu-id="1f275-107">Key resource types</span></span>

| <span data-ttu-id="1f275-108">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1f275-108">Resource</span></span> | <span data-ttu-id="1f275-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1f275-109">Methods</span></span> |
| :-- | :-- |
| [<span data-ttu-id="1f275-110">callRecord</span><span class="sxs-lookup"><span data-stu-id="1f275-110">callRecord</span></span>](callrecords-callrecord.md) | [<span data-ttu-id="1f275-111">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="1f275-111">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |
| [<span data-ttu-id="1f275-112">session</span><span class="sxs-lookup"><span data-stu-id="1f275-112">session</span></span>](callrecords-session.md) | [<span data-ttu-id="1f275-113">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="1f275-113">Get callRecord</span></span>](../api/callrecords-callrecord-get.md)<br />[<span data-ttu-id="1f275-114">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="1f275-114">List sessions</span></span>](../api/callrecords-session-list.md) |
| [<span data-ttu-id="1f275-115">segment</span><span class="sxs-lookup"><span data-stu-id="1f275-115">segment</span></span>](callrecords-segment.md) | [<span data-ttu-id="1f275-116">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="1f275-116">Get callRecord</span></span>](../api/callrecords-callrecord-get.md)<br />[<span data-ttu-id="1f275-117">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="1f275-117">List sessions</span></span>](../api/callrecords-session-list.md) |
| [<span data-ttu-id="1f275-118">pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="1f275-118">pstnCallLogRow</span></span>](callrecords-pstncalllogrow.md)|[<span data-ttu-id="1f275-119">Получение pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="1f275-119">Get pstnCallLogRow</span></span>](../api/callrecords-callrecord-getpstncalls.md) |
| [<span data-ttu-id="1f275-120">directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="1f275-120">directRoutingLogRow</span></span>](callrecords-directroutinglogrow.md) | [<span data-ttu-id="1f275-121">Получение directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="1f275-121">Get directRoutingLogRow</span></span>](../api/callrecords-callrecord-getdirectroutingcalls.md)|

## <a name="call-record-structure"></a><span data-ttu-id="1f275-122">Структура записи звонка</span><span class="sxs-lookup"><span data-stu-id="1f275-122">Call record structure</span></span>

<span data-ttu-id="1f275-123">Объект [callRecord](callrecords-callrecord.md) представляет один одноранговый звонок или групповой звонок между несколькими участниками, иногда называемый собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="1f275-123">The [callRecord](callrecords-callrecord.md) entity represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

<span data-ttu-id="1f275-124">Одноранговый звонок содержит один объект [session](callrecords-session.md)между двумя участниками звонка.</span><span class="sxs-lookup"><span data-stu-id="1f275-124">A peer-to-peer call contains a single [session](callrecords-session.md) between the two participants in the call.</span></span> <span data-ttu-id="1f275-125">Групповые звонки содержат один или несколько объектов **session**.</span><span class="sxs-lookup"><span data-stu-id="1f275-125">Group calls contain one or more **session** entities.</span></span> <span data-ttu-id="1f275-126">В групповом звонке каждый объект **session** находится между участником и конечной точкой службы.</span><span class="sxs-lookup"><span data-stu-id="1f275-126">In a group call, each **session** is between the participant and a service endpoint.</span></span>

<span data-ttu-id="1f275-127">Каждый объект **session** содержит один или несколько объектов [segment](callrecords-segment.md).</span><span class="sxs-lookup"><span data-stu-id="1f275-127">Each **session** contains one or more [segment](callrecords-segment.md) entities.</span></span> <span data-ttu-id="1f275-128">Объект **segment** представляет ссылку на носитель между двумя [конечными точками](callrecords-endpoint.md).</span><span class="sxs-lookup"><span data-stu-id="1f275-128">A **segment** represents a media link between two [endpoints](callrecords-endpoint.md).</span></span> <span data-ttu-id="1f275-129">В большинстве звонков для каждого объекта **session** будет существовать только один объект **segment**, но иногда может иметься одна или несколько промежуточных **конечных точек**.</span><span class="sxs-lookup"><span data-stu-id="1f275-129">For most calls, only one **segment** will be present for each **session**, however sometimes there may be one or more intermediate **endpoints**.</span></span>

![Изображение структуры данных, представляющей полную запись звонка](/graph/images/callrecords-structure.png)

<span data-ttu-id="1f275-131">На схеме выше числа обозначают допустимое количество дочерних элементов каждого типа.</span><span class="sxs-lookup"><span data-stu-id="1f275-131">In the diagram above, the numbers denote how many children of each type can be present.</span></span> <span data-ttu-id="1f275-132">Например, связь 1..N между **callRecord** и **session** означает, что один экземпляр **callRecord** может содержать один или несколько экземпляров **session**.</span><span class="sxs-lookup"><span data-stu-id="1f275-132">For example, a 1..N relationship between a **callRecord** and a **session** means one **callRecord** instance can contain one or more **session** instances.</span></span> <span data-ttu-id="1f275-133">Таким же образом, связь 1..N между **segment** и **media** означает, что один экземпляр **segment** может содержать один или несколько потоков [media](callrecords-media.md).</span><span class="sxs-lookup"><span data-stu-id="1f275-133">Similarly, a 1..N relationship between a **segment** and a **media** means one **segment** instance can contain one or more [media](callrecords-media.md) streams.</span></span>

## <a name="see-also"></a><span data-ttu-id="1f275-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1f275-134">See also</span></span>

- [<span data-ttu-id="1f275-135">Подписки веб-перехватчиков</span><span class="sxs-lookup"><span data-stu-id="1f275-135">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-beta)
