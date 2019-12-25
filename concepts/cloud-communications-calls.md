---
title: Общие сведения о вызовах
description: Узнайте о поддерживаемых типах звонков и о том, как они используются для обработки сигналов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 8de1f5d890504d9edc63213333f1ea8c4b47282f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871675"
---
# <a name="calls-overview"></a><span data-ttu-id="3c38a-103">Общие сведения о вызовах</span><span class="sxs-lookup"><span data-stu-id="3c38a-103">Calls overview</span></span>

<span data-ttu-id="3c38a-104">API облачных коммуникаций в Microsoft Graph добавляют новое измерение, в соответствии с которыми ваши приложения и службы взаимодействуют с пользователями с помощью различных функций, связанных с взаимодействием, таких как звонки и собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="3c38a-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calls and online meetings.</span></span> <span data-ttu-id="3c38a-105">В этой статье описываются поддерживаемые типы звонков и их использование для обработки сигналов.</span><span class="sxs-lookup"><span data-stu-id="3c38a-105">This article describes the supported call types and how they're used for the signaling process.</span></span>

## <a name="peer-to-peer-calls"></a><span data-ttu-id="3c38a-106">Одноранговые вызовы</span><span class="sxs-lookup"><span data-stu-id="3c38a-106">Peer-to-peer calls</span></span>
<span data-ttu-id="3c38a-107">Вызов — Peer-to-Peer (P2P), когда один участник напрямую вызывает другого участника.</span><span class="sxs-lookup"><span data-stu-id="3c38a-107">A call is peer-to-peer (P2P) when one participant is directly calling another participant.</span></span> <span data-ttu-id="3c38a-108">Если элемент Bot вызывает пользователя, а пользователь является единственным выбранным абонентом, это пример вызова P2P.</span><span class="sxs-lookup"><span data-stu-id="3c38a-108">If a bot calls a user, and the user is the only calling target specified, this is an example of a P2P call.</span></span>

![Схема вызовов P2P](images/communications-p2p-call.PNG)

<span data-ttu-id="3c38a-110">Если пользователю требуется позвонить в Bot, для него не требуются дополнительные разрешения для ответа на вызов P2P.</span><span class="sxs-lookup"><span data-stu-id="3c38a-110">If a user wants to call a bot, the bot doesn't need any additional permissions in order to respond to the P2P call.</span></span> <span data-ttu-id="3c38a-111">Чтобы элемент Bot мог вызывать пользователя, он должен иметь разрешение Calls. initiate для вызова P2P.</span><span class="sxs-lookup"><span data-stu-id="3c38a-111">In order for a bot to call a user, it must have the Calls.Initiate.All permission for a P2P call.</span></span>

## <a name="group-calls"></a><span data-ttu-id="3c38a-112">Групповые вызовы</span><span class="sxs-lookup"><span data-stu-id="3c38a-112">Group calls</span></span>

<span data-ttu-id="3c38a-113">Вызов группы происходит, если в вызове есть три или более участника, или если при первоначальном создании вызова были указаны [координаты собрания](/graph/api/resources/onlinemeeting) .</span><span class="sxs-lookup"><span data-stu-id="3c38a-113">A group call occurs if there are either three or more participants in the call, or if [meeting coordinates](/graph/api/resources/onlinemeeting) were specified when the call was initially created.</span></span> 

<span data-ttu-id="3c38a-114">Например, вы можете создать групповой вызов с помощью Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3c38a-114">You can create a group call through Microsoft Teams, for example.</span></span>

![Схема групповых вызовов](images/communications-group-call.PNG)

<span data-ttu-id="3c38a-116">В настоящее время Боты могут выполнять следующие действия:</span><span class="sxs-lookup"><span data-stu-id="3c38a-116">Currently, bots are able to:</span></span>
- <span data-ttu-id="3c38a-117">Создание групповых вызовов</span><span class="sxs-lookup"><span data-stu-id="3c38a-117">Create group calls</span></span>
- <span data-ttu-id="3c38a-118">Присоединение к существующей группе вызовов</span><span class="sxs-lookup"><span data-stu-id="3c38a-118">Join exisiting group calls</span></span>
- <span data-ttu-id="3c38a-119">Приглашение других участников в существующий групповой вызов</span><span class="sxs-lookup"><span data-stu-id="3c38a-119">Invite other participants into an existing group call</span></span>
- <span data-ttu-id="3c38a-120">Приглашать в существующие вызовы групп</span><span class="sxs-lookup"><span data-stu-id="3c38a-120">Be invited into existing group calls</span></span>

## <a name="see-also"></a><span data-ttu-id="3c38a-121">См. также</span><span class="sxs-lookup"><span data-stu-id="3c38a-121">See also</span></span>

- [<span data-ttu-id="3c38a-122">Общие сведения об API облачных коммуникаций</span><span class="sxs-lookup"><span data-stu-id="3c38a-122">Cloud communications API overview</span></span>](cloud-communications-concept-overview.md)
- [<span data-ttu-id="3c38a-123">Разрешения для вызовов</span><span class="sxs-lookup"><span data-stu-id="3c38a-123">Permissions for calls</span></span>](/graph/permissions-reference#calls-permissions)
