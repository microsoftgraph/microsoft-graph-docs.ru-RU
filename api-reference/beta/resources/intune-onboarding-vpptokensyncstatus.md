---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c493a1e967091627504b784cfb7692931af0264e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958524"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="6003a-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="6003a-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="6003a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6003a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6003a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6003a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6003a-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6003a-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="6003a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6003a-107">Members</span></span>
|<span data-ttu-id="6003a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6003a-108">Member</span></span>|<span data-ttu-id="6003a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6003a-109">Value</span></span>|<span data-ttu-id="6003a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6003a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6003a-111">none</span><span class="sxs-lookup"><span data-stu-id="6003a-111">none</span></span>|<span data-ttu-id="6003a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6003a-112">0</span></span>|<span data-ttu-id="6003a-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6003a-113">Default status.</span></span>|
|<span data-ttu-id="6003a-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="6003a-114">inProgress</span></span>|<span data-ttu-id="6003a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="6003a-115">1</span></span>|<span data-ttu-id="6003a-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="6003a-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="6003a-117">готовы</span><span class="sxs-lookup"><span data-stu-id="6003a-117">completed</span></span>|<span data-ttu-id="6003a-118">2</span><span class="sxs-lookup"><span data-stu-id="6003a-118">2</span></span>|<span data-ttu-id="6003a-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="6003a-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="6003a-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="6003a-120">failed</span></span>|<span data-ttu-id="6003a-121">4</span><span class="sxs-lookup"><span data-stu-id="6003a-121">3</span></span>|<span data-ttu-id="6003a-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="6003a-122">Last Sync failed.</span></span>|





