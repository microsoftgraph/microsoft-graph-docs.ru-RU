---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f070740db5b35f32f1ceb3eabeabcd4d8c3a1c9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039477"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="25b66-103">тип перечисления Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="25b66-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="25b66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25b66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25b66-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25b66-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25b66-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25b66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b66-107">Текущее состояние соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="25b66-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="25b66-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="25b66-108">Members</span></span>
|<span data-ttu-id="25b66-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="25b66-109">Member</span></span>|<span data-ttu-id="25b66-110">Значение</span><span class="sxs-lookup"><span data-stu-id="25b66-110">Value</span></span>|<span data-ttu-id="25b66-111">Описание</span><span class="sxs-lookup"><span data-stu-id="25b66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b66-112">нотонбоардед</span><span class="sxs-lookup"><span data-stu-id="25b66-112">notOnboarded</span></span>|<span data-ttu-id="25b66-113">нуль</span><span class="sxs-lookup"><span data-stu-id="25b66-113">0</span></span>|<span data-ttu-id="25b66-114">Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="25b66-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="25b66-115">входящей миграции</span><span class="sxs-lookup"><span data-stu-id="25b66-115">onboarding</span></span>|<span data-ttu-id="25b66-116">1 </span><span class="sxs-lookup"><span data-stu-id="25b66-116">1</span></span>|<span data-ttu-id="25b66-117">Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя</span><span class="sxs-lookup"><span data-stu-id="25b66-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="25b66-118">подключены</span><span class="sxs-lookup"><span data-stu-id="25b66-118">onboarded</span></span>|<span data-ttu-id="25b66-119">2 </span><span class="sxs-lookup"><span data-stu-id="25b66-119">2</span></span>|<span data-ttu-id="25b66-120">Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами</span><span class="sxs-lookup"><span data-stu-id="25b66-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|






