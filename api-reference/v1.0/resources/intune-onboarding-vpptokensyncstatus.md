---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e011f124dbddbcd3bb75a2b1aaf3a83b8dd04a29
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441716"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="e9849-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="e9849-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="e9849-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9849-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9849-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9849-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9849-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="e9849-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="e9849-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="e9849-107">Members</span></span>
|<span data-ttu-id="e9849-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="e9849-108">Member</span></span>|<span data-ttu-id="e9849-109">Значение</span><span class="sxs-lookup"><span data-stu-id="e9849-109">Value</span></span>|<span data-ttu-id="e9849-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e9849-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9849-111">Нет</span><span class="sxs-lookup"><span data-stu-id="e9849-111">none</span></span>|<span data-ttu-id="e9849-112">нуль</span><span class="sxs-lookup"><span data-stu-id="e9849-112">0</span></span>|<span data-ttu-id="e9849-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e9849-113">Default status.</span></span>|
|<span data-ttu-id="e9849-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="e9849-114">inProgress</span></span>|<span data-ttu-id="e9849-115">1,1</span><span class="sxs-lookup"><span data-stu-id="e9849-115">1</span></span>|<span data-ttu-id="e9849-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="e9849-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="e9849-117">готовы</span><span class="sxs-lookup"><span data-stu-id="e9849-117">completed</span></span>|<span data-ttu-id="e9849-118">2</span><span class="sxs-lookup"><span data-stu-id="e9849-118">2</span></span>|<span data-ttu-id="e9849-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="e9849-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="e9849-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="e9849-120">failed</span></span>|<span data-ttu-id="e9849-121">4</span><span class="sxs-lookup"><span data-stu-id="e9849-121">3</span></span>|<span data-ttu-id="e9849-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="e9849-122">Last Sync failed.</span></span>|







