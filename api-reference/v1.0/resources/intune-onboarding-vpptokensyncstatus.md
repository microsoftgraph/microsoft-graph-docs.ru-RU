---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7af4ed87234dc588a9d0969d2ed347adaa4d29da
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037233"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="f8cf7-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="f8cf7-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="f8cf7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8cf7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8cf7-105">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f8cf7-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="f8cf7-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="f8cf7-106">Members</span></span>
|<span data-ttu-id="f8cf7-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="f8cf7-107">Member</span></span>|<span data-ttu-id="f8cf7-108">Значение</span><span class="sxs-lookup"><span data-stu-id="f8cf7-108">Value</span></span>|<span data-ttu-id="f8cf7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f8cf7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8cf7-110">none</span><span class="sxs-lookup"><span data-stu-id="f8cf7-110">none</span></span>|<span data-ttu-id="f8cf7-111">нуль</span><span class="sxs-lookup"><span data-stu-id="f8cf7-111">0</span></span>|<span data-ttu-id="f8cf7-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8cf7-112">Default status.</span></span>|
|<span data-ttu-id="f8cf7-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="f8cf7-113">inProgress</span></span>|<span data-ttu-id="f8cf7-114">1,1</span><span class="sxs-lookup"><span data-stu-id="f8cf7-114">1</span></span>|<span data-ttu-id="f8cf7-115">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="f8cf7-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="f8cf7-116">готовы</span><span class="sxs-lookup"><span data-stu-id="f8cf7-116">completed</span></span>|<span data-ttu-id="f8cf7-117">2</span><span class="sxs-lookup"><span data-stu-id="f8cf7-117">2</span></span>|<span data-ttu-id="f8cf7-118">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="f8cf7-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="f8cf7-119">сбоев</span><span class="sxs-lookup"><span data-stu-id="f8cf7-119">failed</span></span>|<span data-ttu-id="f8cf7-120">4</span><span class="sxs-lookup"><span data-stu-id="f8cf7-120">3</span></span>|<span data-ttu-id="f8cf7-121">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="f8cf7-121">Last Sync failed.</span></span>|



