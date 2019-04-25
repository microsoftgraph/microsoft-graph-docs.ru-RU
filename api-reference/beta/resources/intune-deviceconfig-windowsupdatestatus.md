---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73cd3208b7729544d6fbd620a13ce295b39aff26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523625"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="f8a14-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="f8a14-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="f8a14-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8a14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8a14-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8a14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8a14-106">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="f8a14-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="f8a14-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f8a14-107">Members</span></span>
|<span data-ttu-id="f8a14-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f8a14-108">Member</span></span>|<span data-ttu-id="f8a14-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f8a14-109">Value</span></span>|<span data-ttu-id="f8a14-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f8a14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8a14-111">Уптодате</span><span class="sxs-lookup"><span data-stu-id="f8a14-111">upToDate</span></span>|<span data-ttu-id="f8a14-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f8a14-112">0</span></span>|<span data-ttu-id="f8a14-113">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="f8a14-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="f8a14-114">Пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="f8a14-114">pendingInstallation</span></span>|<span data-ttu-id="f8a14-115">1 </span><span class="sxs-lookup"><span data-stu-id="f8a14-115">1</span></span>|<span data-ttu-id="f8a14-116">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="f8a14-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="f8a14-117">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="f8a14-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="f8a14-118">Пендингребут</span><span class="sxs-lookup"><span data-stu-id="f8a14-118">pendingReboot</span></span>|<span data-ttu-id="f8a14-119">2 </span><span class="sxs-lookup"><span data-stu-id="f8a14-119">2</span></span>|<span data-ttu-id="f8a14-120">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="f8a14-120">There are updates that requires reboot.</span></span> <span data-ttu-id="f8a14-121">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="f8a14-121">There are not failed updates.</span></span>|
|<span data-ttu-id="f8a14-122">сбоев</span><span class="sxs-lookup"><span data-stu-id="f8a14-122">failed</span></span>|<span data-ttu-id="f8a14-123">3 </span><span class="sxs-lookup"><span data-stu-id="f8a14-123">3</span></span>|<span data-ttu-id="f8a14-124">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f8a14-124">There are updates failed to install on the device.</span></span>|





