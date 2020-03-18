---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ac34352ff19bcb9273e638223e87e7f46aad6777
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786160"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="edc12-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="edc12-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="edc12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edc12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edc12-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edc12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edc12-106">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="edc12-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="edc12-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="edc12-107">Members</span></span>
|<span data-ttu-id="edc12-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="edc12-108">Member</span></span>|<span data-ttu-id="edc12-109">Значение</span><span class="sxs-lookup"><span data-stu-id="edc12-109">Value</span></span>|<span data-ttu-id="edc12-110">Описание</span><span class="sxs-lookup"><span data-stu-id="edc12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc12-111">уптодате</span><span class="sxs-lookup"><span data-stu-id="edc12-111">upToDate</span></span>|<span data-ttu-id="edc12-112">нуль</span><span class="sxs-lookup"><span data-stu-id="edc12-112">0</span></span>|<span data-ttu-id="edc12-113">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="edc12-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="edc12-114">пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="edc12-114">pendingInstallation</span></span>|<span data-ttu-id="edc12-115">1,1</span><span class="sxs-lookup"><span data-stu-id="edc12-115">1</span></span>|<span data-ttu-id="edc12-116">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="edc12-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="edc12-117">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="edc12-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="edc12-118">пендингребут</span><span class="sxs-lookup"><span data-stu-id="edc12-118">pendingReboot</span></span>|<span data-ttu-id="edc12-119">2</span><span class="sxs-lookup"><span data-stu-id="edc12-119">2</span></span>|<span data-ttu-id="edc12-120">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="edc12-120">There are updates that requires reboot.</span></span> <span data-ttu-id="edc12-121">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="edc12-121">There are not failed updates.</span></span>|
|<span data-ttu-id="edc12-122">сбоев</span><span class="sxs-lookup"><span data-stu-id="edc12-122">failed</span></span>|<span data-ttu-id="edc12-123">4</span><span class="sxs-lookup"><span data-stu-id="edc12-123">3</span></span>|<span data-ttu-id="edc12-124">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="edc12-124">There are updates failed to install on the device.</span></span>|



