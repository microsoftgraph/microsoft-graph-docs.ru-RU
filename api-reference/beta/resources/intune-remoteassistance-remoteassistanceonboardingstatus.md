---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64b8e1f1735890236aed6a9f642d4fa5860e016b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527526"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="66249-103">тип перечисления Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="66249-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="66249-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="66249-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66249-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66249-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66249-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66249-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66249-107">Текущее состояние соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="66249-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="66249-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="66249-108">Members</span></span>
|<span data-ttu-id="66249-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="66249-109">Member</span></span>|<span data-ttu-id="66249-110">Значение</span><span class="sxs-lookup"><span data-stu-id="66249-110">Value</span></span>|<span data-ttu-id="66249-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66249-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66249-112">нотонбоардед</span><span class="sxs-lookup"><span data-stu-id="66249-112">notOnboarded</span></span>|<span data-ttu-id="66249-113">нуль</span><span class="sxs-lookup"><span data-stu-id="66249-113">0</span></span>|<span data-ttu-id="66249-114">Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="66249-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="66249-115">входящей миграции</span><span class="sxs-lookup"><span data-stu-id="66249-115">onboarding</span></span>|<span data-ttu-id="66249-116">1 </span><span class="sxs-lookup"><span data-stu-id="66249-116">1</span></span>|<span data-ttu-id="66249-117">Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя</span><span class="sxs-lookup"><span data-stu-id="66249-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="66249-118">подключены</span><span class="sxs-lookup"><span data-stu-id="66249-118">onboarded</span></span>|<span data-ttu-id="66249-119">2 </span><span class="sxs-lookup"><span data-stu-id="66249-119">2</span></span>|<span data-ttu-id="66249-120">Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами</span><span class="sxs-lookup"><span data-stu-id="66249-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|



