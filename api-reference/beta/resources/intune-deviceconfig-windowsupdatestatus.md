---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ace0b42b09093ce2e9d485271ec607ffd618c9e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978691"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="f9cf9-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="f9cf9-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="f9cf9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9cf9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9cf9-106">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="f9cf9-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="f9cf9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f9cf9-107">Members</span></span>
|<span data-ttu-id="f9cf9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f9cf9-108">Member</span></span>|<span data-ttu-id="f9cf9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f9cf9-109">Value</span></span>|<span data-ttu-id="f9cf9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f9cf9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9cf9-111">Уптодате</span><span class="sxs-lookup"><span data-stu-id="f9cf9-111">upToDate</span></span>|<span data-ttu-id="f9cf9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f9cf9-112">0</span></span>|<span data-ttu-id="f9cf9-113">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="f9cf9-114">Пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="f9cf9-114">pendingInstallation</span></span>|<span data-ttu-id="f9cf9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="f9cf9-115">1</span></span>|<span data-ttu-id="f9cf9-116">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="f9cf9-117">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="f9cf9-118">Пендингребут</span><span class="sxs-lookup"><span data-stu-id="f9cf9-118">pendingReboot</span></span>|<span data-ttu-id="f9cf9-119">2</span><span class="sxs-lookup"><span data-stu-id="f9cf9-119">2</span></span>|<span data-ttu-id="f9cf9-120">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-120">There are updates that requires reboot.</span></span> <span data-ttu-id="f9cf9-121">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-121">There are not failed updates.</span></span>|
|<span data-ttu-id="f9cf9-122">сбоев</span><span class="sxs-lookup"><span data-stu-id="f9cf9-122">failed</span></span>|<span data-ttu-id="f9cf9-123">4</span><span class="sxs-lookup"><span data-stu-id="f9cf9-123">3</span></span>|<span data-ttu-id="f9cf9-124">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f9cf9-124">There are updates failed to install on the device.</span></span>|





