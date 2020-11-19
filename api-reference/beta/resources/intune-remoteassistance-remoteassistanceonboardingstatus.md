---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ccb04964c7608c24ec8822bac7832aaf77bdfd7f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287790"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="63012-103">тип перечисления Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="63012-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="63012-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63012-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63012-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63012-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63012-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63012-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63012-107">Текущее состояние соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="63012-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="63012-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="63012-108">Members</span></span>
|<span data-ttu-id="63012-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="63012-109">Member</span></span>|<span data-ttu-id="63012-110">Значение</span><span class="sxs-lookup"><span data-stu-id="63012-110">Value</span></span>|<span data-ttu-id="63012-111">Описание</span><span class="sxs-lookup"><span data-stu-id="63012-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63012-112">нотонбоардед</span><span class="sxs-lookup"><span data-stu-id="63012-112">notOnboarded</span></span>|<span data-ttu-id="63012-113">нуль</span><span class="sxs-lookup"><span data-stu-id="63012-113">0</span></span>|<span data-ttu-id="63012-114">Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="63012-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="63012-115">входящей миграции</span><span class="sxs-lookup"><span data-stu-id="63012-115">onboarding</span></span>|<span data-ttu-id="63012-116">1,1</span><span class="sxs-lookup"><span data-stu-id="63012-116">1</span></span>|<span data-ttu-id="63012-117">Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя</span><span class="sxs-lookup"><span data-stu-id="63012-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="63012-118">подключены</span><span class="sxs-lookup"><span data-stu-id="63012-118">onboarded</span></span>|<span data-ttu-id="63012-119">2</span><span class="sxs-lookup"><span data-stu-id="63012-119">2</span></span>|<span data-ttu-id="63012-120">Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами</span><span class="sxs-lookup"><span data-stu-id="63012-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|




