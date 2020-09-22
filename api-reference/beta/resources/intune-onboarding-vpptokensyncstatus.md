---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 912c6c2b0039ca5488b6b2d2972bcf27b7e9624d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029339"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="7e3d2-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="7e3d2-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="7e3d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e3d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e3d2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e3d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e3d2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e3d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e3d2-107">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="7e3d2-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="7e3d2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7e3d2-108">Members</span></span>
|<span data-ttu-id="7e3d2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7e3d2-109">Member</span></span>|<span data-ttu-id="7e3d2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7e3d2-110">Value</span></span>|<span data-ttu-id="7e3d2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7e3d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e3d2-112">Нет</span><span class="sxs-lookup"><span data-stu-id="7e3d2-112">none</span></span>|<span data-ttu-id="7e3d2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7e3d2-113">0</span></span>|<span data-ttu-id="7e3d2-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7e3d2-114">Default status.</span></span>|
|<span data-ttu-id="7e3d2-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="7e3d2-115">inProgress</span></span>|<span data-ttu-id="7e3d2-116">1 </span><span class="sxs-lookup"><span data-stu-id="7e3d2-116">1</span></span>|<span data-ttu-id="7e3d2-117">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="7e3d2-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="7e3d2-118">готовы</span><span class="sxs-lookup"><span data-stu-id="7e3d2-118">completed</span></span>|<span data-ttu-id="7e3d2-119">2 </span><span class="sxs-lookup"><span data-stu-id="7e3d2-119">2</span></span>|<span data-ttu-id="7e3d2-120">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="7e3d2-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="7e3d2-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="7e3d2-121">failed</span></span>|<span data-ttu-id="7e3d2-122">4</span><span class="sxs-lookup"><span data-stu-id="7e3d2-122">3</span></span>|<span data-ttu-id="7e3d2-123">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="7e3d2-123">Last Sync failed.</span></span>|






