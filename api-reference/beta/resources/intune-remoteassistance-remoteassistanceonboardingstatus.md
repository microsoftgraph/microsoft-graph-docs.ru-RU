---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a2cd852d115d32b7a2daa007447e4e544d300ffa
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178789"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="b4676-103">тип перечисления Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="b4676-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="b4676-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4676-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4676-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4676-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4676-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4676-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4676-107">Текущее состояние соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="b4676-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="b4676-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b4676-108">Members</span></span>
|<span data-ttu-id="b4676-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b4676-109">Member</span></span>|<span data-ttu-id="b4676-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b4676-110">Value</span></span>|<span data-ttu-id="b4676-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b4676-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4676-112">нотонбоардед</span><span class="sxs-lookup"><span data-stu-id="b4676-112">notOnboarded</span></span>|<span data-ttu-id="b4676-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b4676-113">0</span></span>|<span data-ttu-id="b4676-114">Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="b4676-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="b4676-115">входящей миграции</span><span class="sxs-lookup"><span data-stu-id="b4676-115">onboarding</span></span>|<span data-ttu-id="b4676-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b4676-116">1</span></span>|<span data-ttu-id="b4676-117">Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя</span><span class="sxs-lookup"><span data-stu-id="b4676-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="b4676-118">подключены</span><span class="sxs-lookup"><span data-stu-id="b4676-118">onboarded</span></span>|<span data-ttu-id="b4676-119">2</span><span class="sxs-lookup"><span data-stu-id="b4676-119">2</span></span>|<span data-ttu-id="b4676-120">Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами</span><span class="sxs-lookup"><span data-stu-id="b4676-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|



