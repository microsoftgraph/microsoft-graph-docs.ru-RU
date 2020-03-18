---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68e5a8bff7f1753540a2716a00fd9148e188d7ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772939"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="e276a-103">тип перечисления Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="e276a-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="e276a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e276a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e276a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e276a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e276a-106">Текущее состояние соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="e276a-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="e276a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e276a-107">Members</span></span>
|<span data-ttu-id="e276a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e276a-108">Member</span></span>|<span data-ttu-id="e276a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e276a-109">Value</span></span>|<span data-ttu-id="e276a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e276a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e276a-111">нотонбоардед</span><span class="sxs-lookup"><span data-stu-id="e276a-111">notOnboarded</span></span>|<span data-ttu-id="e276a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e276a-112">0</span></span>|<span data-ttu-id="e276a-113">Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="e276a-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="e276a-114">входящей миграции</span><span class="sxs-lookup"><span data-stu-id="e276a-114">onboarding</span></span>|<span data-ttu-id="e276a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e276a-115">1</span></span>|<span data-ttu-id="e276a-116">Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя</span><span class="sxs-lookup"><span data-stu-id="e276a-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="e276a-117">подключены</span><span class="sxs-lookup"><span data-stu-id="e276a-117">onboarded</span></span>|<span data-ttu-id="e276a-118">2</span><span class="sxs-lookup"><span data-stu-id="e276a-118">2</span></span>|<span data-ttu-id="e276a-119">Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами</span><span class="sxs-lookup"><span data-stu-id="e276a-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|



