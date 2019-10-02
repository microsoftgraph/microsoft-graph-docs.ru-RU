---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5475a49341005b3c5d8037cc1697b84ce9be57f6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360687"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="a6d44-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="a6d44-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="a6d44-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6d44-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6d44-105">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a6d44-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="a6d44-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="a6d44-106">Members</span></span>
|<span data-ttu-id="a6d44-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="a6d44-107">Member</span></span>|<span data-ttu-id="a6d44-108">Значение</span><span class="sxs-lookup"><span data-stu-id="a6d44-108">Value</span></span>|<span data-ttu-id="a6d44-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a6d44-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6d44-110">none</span><span class="sxs-lookup"><span data-stu-id="a6d44-110">none</span></span>|<span data-ttu-id="a6d44-111">нуль</span><span class="sxs-lookup"><span data-stu-id="a6d44-111">0</span></span>|<span data-ttu-id="a6d44-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a6d44-112">Default status.</span></span>|
|<span data-ttu-id="a6d44-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="a6d44-113">inProgress</span></span>|<span data-ttu-id="a6d44-114">1,1</span><span class="sxs-lookup"><span data-stu-id="a6d44-114">1</span></span>|<span data-ttu-id="a6d44-115">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="a6d44-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="a6d44-116">готовы</span><span class="sxs-lookup"><span data-stu-id="a6d44-116">completed</span></span>|<span data-ttu-id="a6d44-117">2</span><span class="sxs-lookup"><span data-stu-id="a6d44-117">2</span></span>|<span data-ttu-id="a6d44-118">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="a6d44-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="a6d44-119">сбоев</span><span class="sxs-lookup"><span data-stu-id="a6d44-119">failed</span></span>|<span data-ttu-id="a6d44-120">4</span><span class="sxs-lookup"><span data-stu-id="a6d44-120">3</span></span>|<span data-ttu-id="a6d44-121">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="a6d44-121">Last Sync failed.</span></span>|




