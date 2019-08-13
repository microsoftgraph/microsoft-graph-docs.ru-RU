---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd51496000bce906457b4ea03586a41c46e2e426
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308150"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="e538e-103">тип перечисления Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="e538e-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="e538e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e538e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e538e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e538e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e538e-106">Текущее состояние соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="e538e-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="e538e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e538e-107">Members</span></span>
|<span data-ttu-id="e538e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e538e-108">Member</span></span>|<span data-ttu-id="e538e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e538e-109">Value</span></span>|<span data-ttu-id="e538e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e538e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e538e-111">нотонбоардед</span><span class="sxs-lookup"><span data-stu-id="e538e-111">notOnboarded</span></span>|<span data-ttu-id="e538e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e538e-112">0</span></span>|<span data-ttu-id="e538e-113">Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="e538e-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="e538e-114">входящей миграции</span><span class="sxs-lookup"><span data-stu-id="e538e-114">onboarding</span></span>|<span data-ttu-id="e538e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e538e-115">1</span></span>|<span data-ttu-id="e538e-116">Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя</span><span class="sxs-lookup"><span data-stu-id="e538e-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="e538e-117">подключены</span><span class="sxs-lookup"><span data-stu-id="e538e-117">onboarded</span></span>|<span data-ttu-id="e538e-118">2</span><span class="sxs-lookup"><span data-stu-id="e538e-118">2</span></span>|<span data-ttu-id="e538e-119">Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами</span><span class="sxs-lookup"><span data-stu-id="e538e-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|



