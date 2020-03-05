---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0d17b599460a5d7b6a7e37f7255f050df8350ccd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447992"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="92a90-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="92a90-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="92a90-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92a90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92a90-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92a90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92a90-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="92a90-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="92a90-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="92a90-107">Members</span></span>
|<span data-ttu-id="92a90-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="92a90-108">Member</span></span>|<span data-ttu-id="92a90-109">Значение</span><span class="sxs-lookup"><span data-stu-id="92a90-109">Value</span></span>|<span data-ttu-id="92a90-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92a90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a90-111">нет</span><span class="sxs-lookup"><span data-stu-id="92a90-111">none</span></span>|<span data-ttu-id="92a90-112">нуль</span><span class="sxs-lookup"><span data-stu-id="92a90-112">0</span></span>|<span data-ttu-id="92a90-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="92a90-113">Default status.</span></span>|
|<span data-ttu-id="92a90-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="92a90-114">inProgress</span></span>|<span data-ttu-id="92a90-115">1 </span><span class="sxs-lookup"><span data-stu-id="92a90-115">1</span></span>|<span data-ttu-id="92a90-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="92a90-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="92a90-117">готовы</span><span class="sxs-lookup"><span data-stu-id="92a90-117">completed</span></span>|<span data-ttu-id="92a90-118">2 </span><span class="sxs-lookup"><span data-stu-id="92a90-118">2</span></span>|<span data-ttu-id="92a90-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="92a90-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="92a90-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="92a90-120">failed</span></span>|<span data-ttu-id="92a90-121">3 </span><span class="sxs-lookup"><span data-stu-id="92a90-121">3</span></span>|<span data-ttu-id="92a90-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="92a90-122">Last Sync failed.</span></span>|




