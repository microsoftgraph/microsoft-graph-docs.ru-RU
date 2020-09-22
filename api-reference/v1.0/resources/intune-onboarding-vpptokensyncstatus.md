---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ba530475e03a2aef3b34d5387fc61d500fc94585
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025250"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="7b649-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="7b649-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="7b649-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b649-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b649-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b649-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="7b649-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="7b649-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7b649-107">Members</span></span>
|<span data-ttu-id="7b649-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7b649-108">Member</span></span>|<span data-ttu-id="7b649-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7b649-109">Value</span></span>|<span data-ttu-id="7b649-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b649-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b649-111">Нет</span><span class="sxs-lookup"><span data-stu-id="7b649-111">none</span></span>|<span data-ttu-id="7b649-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7b649-112">0</span></span>|<span data-ttu-id="7b649-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7b649-113">Default status.</span></span>|
|<span data-ttu-id="7b649-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="7b649-114">inProgress</span></span>|<span data-ttu-id="7b649-115">1 </span><span class="sxs-lookup"><span data-stu-id="7b649-115">1</span></span>|<span data-ttu-id="7b649-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="7b649-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="7b649-117">готовы</span><span class="sxs-lookup"><span data-stu-id="7b649-117">completed</span></span>|<span data-ttu-id="7b649-118">2 </span><span class="sxs-lookup"><span data-stu-id="7b649-118">2</span></span>|<span data-ttu-id="7b649-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="7b649-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="7b649-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="7b649-120">failed</span></span>|<span data-ttu-id="7b649-121">4</span><span class="sxs-lookup"><span data-stu-id="7b649-121">3</span></span>|<span data-ttu-id="7b649-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="7b649-122">Last Sync failed.</span></span>|









