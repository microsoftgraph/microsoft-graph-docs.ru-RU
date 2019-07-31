---
title: тип перечисления Ремотеассистанцеонбоардингстатус
description: Текущее состояние соединителя TeamViewer Connector
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 40d3c7813088370ddffad2fc787d53c96ad0f70b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967569"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="6b89c-103">тип перечисления Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="6b89c-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="6b89c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b89c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b89c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b89c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b89c-106">Текущее состояние соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="6b89c-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="6b89c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6b89c-107">Members</span></span>
|<span data-ttu-id="6b89c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6b89c-108">Member</span></span>|<span data-ttu-id="6b89c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6b89c-109">Value</span></span>|<span data-ttu-id="6b89c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b89c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b89c-111">Нотонбоардед</span><span class="sxs-lookup"><span data-stu-id="6b89c-111">notOnboarded</span></span>|<span data-ttu-id="6b89c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6b89c-112">0</span></span>|<span data-ttu-id="6b89c-113">Состояние, указанное при отсутствии активного соединителя TeamViewer Connector, настроенного или активного</span><span class="sxs-lookup"><span data-stu-id="6b89c-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="6b89c-114">входящей миграции</span><span class="sxs-lookup"><span data-stu-id="6b89c-114">onboarding</span></span>|<span data-ttu-id="6b89c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="6b89c-115">1</span></span>|<span data-ttu-id="6b89c-116">Сведения о состоянии, когда система инициировала подключение TeamViewer, но служба еще не выполнила подтверждение соединителя</span><span class="sxs-lookup"><span data-stu-id="6b89c-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="6b89c-117">подключены</span><span class="sxs-lookup"><span data-stu-id="6b89c-117">onboarded</span></span>|<span data-ttu-id="6b89c-118">2</span><span class="sxs-lookup"><span data-stu-id="6b89c-118">2</span></span>|<span data-ttu-id="6b89c-119">Состояние, полученное в отчете, когда система успешно выполнила обмен сведениями об учетной записи с TeamViewer, и теперь может инициировать сеансы удаленного помощника с клиентами</span><span class="sxs-lookup"><span data-stu-id="6b89c-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|





