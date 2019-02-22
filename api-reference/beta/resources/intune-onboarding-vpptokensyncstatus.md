---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46de00423a08e7edc6f5ac9c62d1caf0165e1d94
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170429"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="bf6ee-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="bf6ee-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="bf6ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf6ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf6ee-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf6ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf6ee-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="bf6ee-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="bf6ee-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bf6ee-107">Members</span></span>
|<span data-ttu-id="bf6ee-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bf6ee-108">Member</span></span>|<span data-ttu-id="bf6ee-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bf6ee-109">Value</span></span>|<span data-ttu-id="bf6ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bf6ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf6ee-111">Нет</span><span class="sxs-lookup"><span data-stu-id="bf6ee-111">none</span></span>|<span data-ttu-id="bf6ee-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bf6ee-112">0</span></span>|<span data-ttu-id="bf6ee-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bf6ee-113">Default status.</span></span>|
|<span data-ttu-id="bf6ee-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="bf6ee-114">inProgress</span></span>|<span data-ttu-id="bf6ee-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bf6ee-115">1</span></span>|<span data-ttu-id="bf6ee-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="bf6ee-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="bf6ee-117">готовы</span><span class="sxs-lookup"><span data-stu-id="bf6ee-117">completed</span></span>|<span data-ttu-id="bf6ee-118">2</span><span class="sxs-lookup"><span data-stu-id="bf6ee-118">2</span></span>|<span data-ttu-id="bf6ee-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="bf6ee-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="bf6ee-120">failed</span><span class="sxs-lookup"><span data-stu-id="bf6ee-120">failed</span></span>|<span data-ttu-id="bf6ee-121">4</span><span class="sxs-lookup"><span data-stu-id="bf6ee-121">3</span></span>|<span data-ttu-id="bf6ee-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="bf6ee-122">Last Sync failed.</span></span>|




