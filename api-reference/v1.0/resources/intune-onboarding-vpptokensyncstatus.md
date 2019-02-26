---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6938fd41b6cd7c089b08edb629bc1197ec47c2d7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254053"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="d9eb9-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="d9eb9-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="d9eb9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9eb9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9eb9-105">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d9eb9-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="d9eb9-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d9eb9-106">Members</span></span>
|<span data-ttu-id="d9eb9-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d9eb9-107">Member</span></span>|<span data-ttu-id="d9eb9-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d9eb9-108">Value</span></span>|<span data-ttu-id="d9eb9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d9eb9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9eb9-110">Нет</span><span class="sxs-lookup"><span data-stu-id="d9eb9-110">none</span></span>|<span data-ttu-id="d9eb9-111">нуль</span><span class="sxs-lookup"><span data-stu-id="d9eb9-111">0</span></span>|<span data-ttu-id="d9eb9-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d9eb9-112">Default status.</span></span>|
|<span data-ttu-id="d9eb9-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="d9eb9-113">inProgress</span></span>|<span data-ttu-id="d9eb9-114">1,1</span><span class="sxs-lookup"><span data-stu-id="d9eb9-114">1</span></span>|<span data-ttu-id="d9eb9-115">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="d9eb9-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="d9eb9-116">готовы</span><span class="sxs-lookup"><span data-stu-id="d9eb9-116">completed</span></span>|<span data-ttu-id="d9eb9-117">2</span><span class="sxs-lookup"><span data-stu-id="d9eb9-117">2</span></span>|<span data-ttu-id="d9eb9-118">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="d9eb9-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="d9eb9-119">failed</span><span class="sxs-lookup"><span data-stu-id="d9eb9-119">failed</span></span>|<span data-ttu-id="d9eb9-120">4</span><span class="sxs-lookup"><span data-stu-id="d9eb9-120">3</span></span>|<span data-ttu-id="d9eb9-121">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="d9eb9-121">Last Sync failed.</span></span>|



