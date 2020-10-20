---
title: Работа с API записей звонков в Microsoft Graph
description: API записей звонков Microsoft Graph позволяет извлекать данные об использовании и диагностике для звонков и собраний по сети в вашей организации.
author: williamlooney
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 56b81ceb902701c0125cee6e1b0f20087bbeac50
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601582"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a><span data-ttu-id="d3b51-103">Работа с API записей звонков в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d3b51-103">Working with the call records API in Microsoft Graph</span></span>

<span data-ttu-id="d3b51-104">Записи звонков содержат сведения об использовании и диагностике, касающиеся звонков и собраний по сети в вашей организации при применении Microsoft Teams или Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d3b51-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="d3b51-105">Вы можете использовать API записей звонков, чтобы подписаться на записи звонков и искать их по идентификаторам.</span><span class="sxs-lookup"><span data-stu-id="d3b51-105">You can use the call records APIs to subscribe to call records and look up call records by IDs.</span></span>

<span data-ttu-id="d3b51-106">API записи звонков задается в подпространстве имен OData, `microsoft.graph.callRecords`.</span><span class="sxs-lookup"><span data-stu-id="d3b51-106">The call records API is defined in the OData sub-namespace, `microsoft.graph.callRecords`.</span></span>

## <a name="key-resource-types"></a><span data-ttu-id="d3b51-107">Ключевые типы ресурсов</span><span class="sxs-lookup"><span data-stu-id="d3b51-107">Key resource types</span></span>

| <span data-ttu-id="d3b51-108">Ресурс</span><span class="sxs-lookup"><span data-stu-id="d3b51-108">Resource</span></span> | <span data-ttu-id="d3b51-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d3b51-109">Methods</span></span> |
| :-- | :-- |
| [<span data-ttu-id="d3b51-110">callRecord</span><span class="sxs-lookup"><span data-stu-id="d3b51-110">callRecord</span></span>](callrecords-callrecord.md) | [<span data-ttu-id="d3b51-111">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="d3b51-111">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |
| [<span data-ttu-id="d3b51-112">session</span><span class="sxs-lookup"><span data-stu-id="d3b51-112">session</span></span>](callrecords-session.md) | [<span data-ttu-id="d3b51-113">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="d3b51-113">Get callRecord</span></span>](../api/callrecords-callrecord-get.md)<br />[<span data-ttu-id="d3b51-114">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="d3b51-114">List sessions</span></span>](../api/callrecords-session-list.md) |
| [<span data-ttu-id="d3b51-115">segment</span><span class="sxs-lookup"><span data-stu-id="d3b51-115">segment</span></span>](callrecords-segment.md) | [<span data-ttu-id="d3b51-116">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="d3b51-116">Get callRecord</span></span>](../api/callrecords-callrecord-get.md)<br />[<span data-ttu-id="d3b51-117">Перечисление сеансов</span><span class="sxs-lookup"><span data-stu-id="d3b51-117">List sessions</span></span>](../api/callrecords-session-list.md) |

## <a name="call-record-structure"></a><span data-ttu-id="d3b51-118">Структура записи звонка</span><span class="sxs-lookup"><span data-stu-id="d3b51-118">Call record structure</span></span>

<span data-ttu-id="d3b51-119">Объект [callRecord](callrecords-callrecord.md) представляет один одноранговый звонок или групповой звонок между несколькими участниками, иногда называемый собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="d3b51-119">The [callRecord](callrecords-callrecord.md) entity represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

<span data-ttu-id="d3b51-120">Одноранговый звонок содержит один объект [session](callrecords-session.md)между двумя участниками звонка.</span><span class="sxs-lookup"><span data-stu-id="d3b51-120">A peer-to-peer call contains a single [session](callrecords-session.md) between the two participants in the call.</span></span> <span data-ttu-id="d3b51-121">Групповые звонки содержат один или несколько объектов **session**.</span><span class="sxs-lookup"><span data-stu-id="d3b51-121">Group calls contain one or more **session** entities.</span></span> <span data-ttu-id="d3b51-122">В групповом звонке каждый объект **session** находится между участником и конечной точкой службы.</span><span class="sxs-lookup"><span data-stu-id="d3b51-122">In a group call, each **session** is between the participant and a service endpoint.</span></span>

<span data-ttu-id="d3b51-123">Каждый объект **session** содержит один или несколько объектов [segment](callrecords-segment.md).</span><span class="sxs-lookup"><span data-stu-id="d3b51-123">Each **session** contains one or more [segment](callrecords-segment.md) entities.</span></span> <span data-ttu-id="d3b51-124">Объект **segment** представляет ссылку на носитель между двумя [конечными точками](callrecords-endpoint.md).</span><span class="sxs-lookup"><span data-stu-id="d3b51-124">A **segment** represents a media link between two [endpoints](callrecords-endpoint.md).</span></span> <span data-ttu-id="d3b51-125">В большинстве звонков для каждого объекта **session** будет существовать только один объект **segment**, но иногда может иметься одна или несколько промежуточных **конечных точек**.</span><span class="sxs-lookup"><span data-stu-id="d3b51-125">For most calls, only one **segment** will be present for each **session**, however sometimes there may be one or more intermediate **endpoints**.</span></span>

![Изображение структуры данных, представляющей полную запись звонка](/graph/images/callrecords-structure.png)

<span data-ttu-id="d3b51-127">На схеме выше числа обозначают допустимое количество дочерних элементов каждого типа.</span><span class="sxs-lookup"><span data-stu-id="d3b51-127">In the diagram above, the numbers denote how many children of each type can be present.</span></span> <span data-ttu-id="d3b51-128">Например, связь 1..N между **callRecord** и **session** означает, что один экземпляр **callRecord** может содержать один или несколько экземпляров **session**.</span><span class="sxs-lookup"><span data-stu-id="d3b51-128">For example, a 1..N relationship between a **callRecord** and a **session** means one **callRecord** instance can contain one or more **session** instances.</span></span> <span data-ttu-id="d3b51-129">Таким же образом, связь 1..N между **segment** и **media** означает, что один экземпляр **segment** может содержать один или несколько потоков [media](callrecords-media.md).</span><span class="sxs-lookup"><span data-stu-id="d3b51-129">Similarly, a 1..N relationship between a **segment** and a **media** means one **segment** instance can contain one or more [media](callrecords-media.md) streams.</span></span>

## <a name="see-also"></a><span data-ttu-id="d3b51-130">См. также</span><span class="sxs-lookup"><span data-stu-id="d3b51-130">See also</span></span>

- [<span data-ttu-id="d3b51-131">Подписки веб-перехватчиков</span><span class="sxs-lookup"><span data-stu-id="d3b51-131">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-1.0)

