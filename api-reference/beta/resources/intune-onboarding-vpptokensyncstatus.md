---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 27d66ddf8e17072c7df27c63565e83e5d69df7c3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259398"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="7b727-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="7b727-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="7b727-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b727-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b727-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b727-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b727-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b727-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b727-107">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="7b727-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="7b727-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7b727-108">Members</span></span>
|<span data-ttu-id="7b727-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7b727-109">Member</span></span>|<span data-ttu-id="7b727-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7b727-110">Value</span></span>|<span data-ttu-id="7b727-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7b727-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b727-112">Нет</span><span class="sxs-lookup"><span data-stu-id="7b727-112">none</span></span>|<span data-ttu-id="7b727-113">нуль</span><span class="sxs-lookup"><span data-stu-id="7b727-113">0</span></span>|<span data-ttu-id="7b727-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7b727-114">Default status.</span></span>|
|<span data-ttu-id="7b727-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="7b727-115">inProgress</span></span>|<span data-ttu-id="7b727-116">1,1</span><span class="sxs-lookup"><span data-stu-id="7b727-116">1</span></span>|<span data-ttu-id="7b727-117">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="7b727-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="7b727-118">готовы</span><span class="sxs-lookup"><span data-stu-id="7b727-118">completed</span></span>|<span data-ttu-id="7b727-119">2</span><span class="sxs-lookup"><span data-stu-id="7b727-119">2</span></span>|<span data-ttu-id="7b727-120">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="7b727-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="7b727-121">сбоев</span><span class="sxs-lookup"><span data-stu-id="7b727-121">failed</span></span>|<span data-ttu-id="7b727-122">4</span><span class="sxs-lookup"><span data-stu-id="7b727-122">3</span></span>|<span data-ttu-id="7b727-123">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="7b727-123">Last Sync failed.</span></span>|




