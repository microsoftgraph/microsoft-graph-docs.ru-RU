---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a9955b825fffab7837cb2c77ffa443ad3f9c9fa1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524064"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="d5fd2-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="d5fd2-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="d5fd2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d5fd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5fd2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5fd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5fd2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5fd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5fd2-107">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d5fd2-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="d5fd2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d5fd2-108">Members</span></span>
|<span data-ttu-id="d5fd2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d5fd2-109">Member</span></span>|<span data-ttu-id="d5fd2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d5fd2-110">Value</span></span>|<span data-ttu-id="d5fd2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d5fd2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5fd2-112">нет</span><span class="sxs-lookup"><span data-stu-id="d5fd2-112">none</span></span>|<span data-ttu-id="d5fd2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d5fd2-113">0</span></span>|<span data-ttu-id="d5fd2-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d5fd2-114">Default status.</span></span>|
|<span data-ttu-id="d5fd2-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="d5fd2-115">inProgress</span></span>|<span data-ttu-id="d5fd2-116">1 </span><span class="sxs-lookup"><span data-stu-id="d5fd2-116">1</span></span>|<span data-ttu-id="d5fd2-117">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="d5fd2-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="d5fd2-118">готовы</span><span class="sxs-lookup"><span data-stu-id="d5fd2-118">completed</span></span>|<span data-ttu-id="d5fd2-119">2 </span><span class="sxs-lookup"><span data-stu-id="d5fd2-119">2</span></span>|<span data-ttu-id="d5fd2-120">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="d5fd2-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="d5fd2-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="d5fd2-121">failed</span></span>|<span data-ttu-id="d5fd2-122">3 </span><span class="sxs-lookup"><span data-stu-id="d5fd2-122">3</span></span>|<span data-ttu-id="d5fd2-123">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="d5fd2-123">Last Sync failed.</span></span>|



