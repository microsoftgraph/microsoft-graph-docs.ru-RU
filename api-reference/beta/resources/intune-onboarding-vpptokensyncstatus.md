---
title: тип перечисления Впптокенсинкстатус
description: Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ede152d056c082e3b55c9142730ce61af86ae48c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369348"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="20640-103">тип перечисления Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="20640-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="20640-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20640-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20640-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20640-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20640-106">Возможные состояния синхронизации, связанные с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="20640-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="20640-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="20640-107">Members</span></span>
|<span data-ttu-id="20640-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="20640-108">Member</span></span>|<span data-ttu-id="20640-109">Значение</span><span class="sxs-lookup"><span data-stu-id="20640-109">Value</span></span>|<span data-ttu-id="20640-110">Описание</span><span class="sxs-lookup"><span data-stu-id="20640-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20640-111">none</span><span class="sxs-lookup"><span data-stu-id="20640-111">none</span></span>|<span data-ttu-id="20640-112">нуль</span><span class="sxs-lookup"><span data-stu-id="20640-112">0</span></span>|<span data-ttu-id="20640-113">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="20640-113">Default status.</span></span>|
|<span data-ttu-id="20640-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="20640-114">inProgress</span></span>|<span data-ttu-id="20640-115">1,1</span><span class="sxs-lookup"><span data-stu-id="20640-115">1</span></span>|<span data-ttu-id="20640-116">Выполняется Последняя синхронизация.</span><span class="sxs-lookup"><span data-stu-id="20640-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="20640-117">готовы</span><span class="sxs-lookup"><span data-stu-id="20640-117">completed</span></span>|<span data-ttu-id="20640-118">2</span><span class="sxs-lookup"><span data-stu-id="20640-118">2</span></span>|<span data-ttu-id="20640-119">Последняя синхронизация выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="20640-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="20640-120">сбоев</span><span class="sxs-lookup"><span data-stu-id="20640-120">failed</span></span>|<span data-ttu-id="20640-121">4</span><span class="sxs-lookup"><span data-stu-id="20640-121">3</span></span>|<span data-ttu-id="20640-122">Не удалось выполнить последнюю синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="20640-122">Last Sync failed.</span></span>|



