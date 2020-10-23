---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d1539f7692a181e43a932848d3401246c0cab26
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703603"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="a169a-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="a169a-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="a169a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a169a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a169a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a169a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a169a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a169a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a169a-107">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a169a-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="a169a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a169a-108">Members</span></span>
|<span data-ttu-id="a169a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a169a-109">Member</span></span>|<span data-ttu-id="a169a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a169a-110">Value</span></span>|<span data-ttu-id="a169a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a169a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a169a-112">none</span><span class="sxs-lookup"><span data-stu-id="a169a-112">none</span></span>|<span data-ttu-id="a169a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="a169a-113">0</span></span>|<span data-ttu-id="a169a-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a169a-114">Default status.</span></span>|
|<span data-ttu-id="a169a-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="a169a-115">inProgress</span></span>|<span data-ttu-id="a169a-116">1,1</span><span class="sxs-lookup"><span data-stu-id="a169a-116">1</span></span>|<span data-ttu-id="a169a-117">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="a169a-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="a169a-118">готовы</span><span class="sxs-lookup"><span data-stu-id="a169a-118">completed</span></span>|<span data-ttu-id="a169a-119">2</span><span class="sxs-lookup"><span data-stu-id="a169a-119">2</span></span>|<span data-ttu-id="a169a-120">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="a169a-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="a169a-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="a169a-121">failed</span></span>|<span data-ttu-id="a169a-122">4</span><span class="sxs-lookup"><span data-stu-id="a169a-122">3</span></span>|<span data-ttu-id="a169a-123">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="a169a-123">Last Sync failed.</span></span>|





