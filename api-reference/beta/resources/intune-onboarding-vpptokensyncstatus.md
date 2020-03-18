---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b298fd52c390d9e926ca9be69e276aac3b6a6de0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777259"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="4347a-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="4347a-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="4347a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4347a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4347a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4347a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4347a-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="4347a-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="4347a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4347a-107">Members</span></span>
|<span data-ttu-id="4347a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4347a-108">Member</span></span>|<span data-ttu-id="4347a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4347a-109">Value</span></span>|<span data-ttu-id="4347a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4347a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4347a-111">none</span><span class="sxs-lookup"><span data-stu-id="4347a-111">none</span></span>|<span data-ttu-id="4347a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4347a-112">0</span></span>|<span data-ttu-id="4347a-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4347a-113">Default status.</span></span>|
|<span data-ttu-id="4347a-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="4347a-114">inProgress</span></span>|<span data-ttu-id="4347a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="4347a-115">1</span></span>|<span data-ttu-id="4347a-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="4347a-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="4347a-117">готовы</span><span class="sxs-lookup"><span data-stu-id="4347a-117">completed</span></span>|<span data-ttu-id="4347a-118">2</span><span class="sxs-lookup"><span data-stu-id="4347a-118">2</span></span>|<span data-ttu-id="4347a-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="4347a-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="4347a-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="4347a-120">failed</span></span>|<span data-ttu-id="4347a-121">4</span><span class="sxs-lookup"><span data-stu-id="4347a-121">3</span></span>|<span data-ttu-id="4347a-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="4347a-122">Last Sync failed.</span></span>|



