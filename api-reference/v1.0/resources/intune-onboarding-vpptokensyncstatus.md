---
title: тип enum vppTokenSyncStatus
description: Возможные состояния синхронизации, связанные с маркером программы покупки тома Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1468240f5d83002d21336299486bceca259a207f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755695"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="4f3a4-103">тип enum vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="4f3a4-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="4f3a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f3a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f3a4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f3a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f3a4-106">Возможные состояния синхронизации, связанные с маркером программы покупки тома Apple.</span><span class="sxs-lookup"><span data-stu-id="4f3a4-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="4f3a4-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4f3a4-107">Members</span></span>
|<span data-ttu-id="4f3a4-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4f3a4-108">Member</span></span>|<span data-ttu-id="4f3a4-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4f3a4-109">Value</span></span>|<span data-ttu-id="4f3a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f3a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f3a4-111">нет</span><span class="sxs-lookup"><span data-stu-id="4f3a4-111">none</span></span>|<span data-ttu-id="4f3a4-112">0</span><span class="sxs-lookup"><span data-stu-id="4f3a4-112">0</span></span>|<span data-ttu-id="4f3a4-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f3a4-113">Default status.</span></span>|
|<span data-ttu-id="4f3a4-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="4f3a4-114">inProgress</span></span>|<span data-ttu-id="4f3a4-115">1</span><span class="sxs-lookup"><span data-stu-id="4f3a4-115">1</span></span>|<span data-ttu-id="4f3a4-116">Последняя синхронизация в процессе.</span><span class="sxs-lookup"><span data-stu-id="4f3a4-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="4f3a4-117">завершено</span><span class="sxs-lookup"><span data-stu-id="4f3a4-117">completed</span></span>|<span data-ttu-id="4f3a4-118">2</span><span class="sxs-lookup"><span data-stu-id="4f3a4-118">2</span></span>|<span data-ttu-id="4f3a4-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="4f3a4-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="4f3a4-120">не удалось</span><span class="sxs-lookup"><span data-stu-id="4f3a4-120">failed</span></span>|<span data-ttu-id="4f3a4-121">3</span><span class="sxs-lookup"><span data-stu-id="4f3a4-121">3</span></span>|<span data-ttu-id="4f3a4-122">Последняя синхронизация не удалась.</span><span class="sxs-lookup"><span data-stu-id="4f3a4-122">Last Sync failed.</span></span>|




