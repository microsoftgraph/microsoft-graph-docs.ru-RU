---
title: тип переименовки remoteAssistanceOnboardingStatus
description: Текущее состояние соединиттеля TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d63300e02f1442a38bbcda7f8e211e9356b8e57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755681"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="8ac38-103">тип переименовки remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="8ac38-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="8ac38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ac38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ac38-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ac38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ac38-106">Текущее состояние соединиттеля TeamViewer</span><span class="sxs-lookup"><span data-stu-id="8ac38-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="8ac38-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8ac38-107">Members</span></span>
|<span data-ttu-id="8ac38-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8ac38-108">Member</span></span>|<span data-ttu-id="8ac38-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8ac38-109">Value</span></span>|<span data-ttu-id="8ac38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8ac38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ac38-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="8ac38-111">notOnboarded</span></span>|<span data-ttu-id="8ac38-112">0</span><span class="sxs-lookup"><span data-stu-id="8ac38-112">0</span></span>|<span data-ttu-id="8ac38-113">Состояние, сообщаемое при отсутствие активного соединитетеля TeamViewer, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="8ac38-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="8ac38-114">onboarding</span><span class="sxs-lookup"><span data-stu-id="8ac38-114">onboarding</span></span>|<span data-ttu-id="8ac38-115">1</span><span class="sxs-lookup"><span data-stu-id="8ac38-115">1</span></span>|<span data-ttu-id="8ac38-116">Состояние, сообщалось, когда система инициировала подключение TeamViewer, но служба еще не завершила подтверждение соединитетеля</span><span class="sxs-lookup"><span data-stu-id="8ac38-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="8ac38-117">onboarded</span><span class="sxs-lookup"><span data-stu-id="8ac38-117">onboarded</span></span>|<span data-ttu-id="8ac38-118">2</span><span class="sxs-lookup"><span data-stu-id="8ac38-118">2</span></span>|<span data-ttu-id="8ac38-119">Состояние, о чем сообщалось, когда система успешно обменивалась сведениями о учетных записях с TeamViewer и теперь может инициировать сеансы удаленной помощи с клиентами</span><span class="sxs-lookup"><span data-stu-id="8ac38-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|




