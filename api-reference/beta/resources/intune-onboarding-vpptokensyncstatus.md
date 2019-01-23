---
title: Тип перечисления vppTokenSyncStatus
description: Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a53906018d45181bd16750e4ed3f0dac9dcb0d1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398816"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="b2ab1-103">Тип перечисления vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b2ab1-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="b2ab1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b2ab1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2ab1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2ab1-107">Возможности синхронизации статусов связанный с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="b2ab1-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b2ab1-108">Members</span></span>
|<span data-ttu-id="b2ab1-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b2ab1-109">Member</span></span>|<span data-ttu-id="b2ab1-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b2ab1-110">Value</span></span>|<span data-ttu-id="b2ab1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2ab1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2ab1-112">none</span><span class="sxs-lookup"><span data-stu-id="b2ab1-112">none</span></span>|<span data-ttu-id="b2ab1-113">0</span><span class="sxs-lookup"><span data-stu-id="b2ab1-113">0</span></span>|<span data-ttu-id="b2ab1-114">Состояние по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-114">Default status.</span></span>|
|<span data-ttu-id="b2ab1-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="b2ab1-115">inProgress</span></span>|<span data-ttu-id="b2ab1-116">1</span><span class="sxs-lookup"><span data-stu-id="b2ab1-116">1</span></span>|<span data-ttu-id="b2ab1-117">Последняя синхронизация в стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="b2ab1-118">завершена</span><span class="sxs-lookup"><span data-stu-id="b2ab1-118">completed</span></span>|<span data-ttu-id="b2ab1-119">2</span><span class="sxs-lookup"><span data-stu-id="b2ab1-119">2</span></span>|<span data-ttu-id="b2ab1-120">Последняя синхронизация успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="b2ab1-121">failed</span><span class="sxs-lookup"><span data-stu-id="b2ab1-121">failed</span></span>|<span data-ttu-id="b2ab1-122">3</span><span class="sxs-lookup"><span data-stu-id="b2ab1-122">3</span></span>|<span data-ttu-id="b2ab1-123">Не удалось последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b2ab1-123">Last Sync failed.</span></span>|




