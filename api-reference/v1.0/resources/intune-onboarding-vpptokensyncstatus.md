---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6938fd41b6cd7c089b08edb629bc1197ec47c2d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548091"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="17cc0-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="17cc0-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="17cc0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17cc0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17cc0-105">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="17cc0-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="17cc0-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="17cc0-106">Members</span></span>
|<span data-ttu-id="17cc0-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="17cc0-107">Member</span></span>|<span data-ttu-id="17cc0-108">Значение</span><span class="sxs-lookup"><span data-stu-id="17cc0-108">Value</span></span>|<span data-ttu-id="17cc0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="17cc0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17cc0-110">Нет</span><span class="sxs-lookup"><span data-stu-id="17cc0-110">none</span></span>|<span data-ttu-id="17cc0-111">нуль</span><span class="sxs-lookup"><span data-stu-id="17cc0-111">0</span></span>|<span data-ttu-id="17cc0-112">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="17cc0-112">Default status.</span></span>|
|<span data-ttu-id="17cc0-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="17cc0-113">inProgress</span></span>|<span data-ttu-id="17cc0-114">1 </span><span class="sxs-lookup"><span data-stu-id="17cc0-114">1</span></span>|<span data-ttu-id="17cc0-115">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="17cc0-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="17cc0-116">готовы</span><span class="sxs-lookup"><span data-stu-id="17cc0-116">completed</span></span>|<span data-ttu-id="17cc0-117">2 </span><span class="sxs-lookup"><span data-stu-id="17cc0-117">2</span></span>|<span data-ttu-id="17cc0-118">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="17cc0-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="17cc0-119">сбоев</span><span class="sxs-lookup"><span data-stu-id="17cc0-119">failed</span></span>|<span data-ttu-id="17cc0-120">3 </span><span class="sxs-lookup"><span data-stu-id="17cc0-120">3</span></span>|<span data-ttu-id="17cc0-121">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="17cc0-121">Last Sync failed.</span></span>|



