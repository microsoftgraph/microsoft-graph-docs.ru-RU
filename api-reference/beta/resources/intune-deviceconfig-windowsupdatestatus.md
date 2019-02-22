---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7549fb77cf5a9f7c3014192d5524019323405f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154161"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="9948a-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="9948a-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="9948a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9948a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9948a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9948a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9948a-106">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="9948a-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="9948a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="9948a-107">Members</span></span>
|<span data-ttu-id="9948a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="9948a-108">Member</span></span>|<span data-ttu-id="9948a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="9948a-109">Value</span></span>|<span data-ttu-id="9948a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9948a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9948a-111">Уптодате</span><span class="sxs-lookup"><span data-stu-id="9948a-111">upToDate</span></span>|<span data-ttu-id="9948a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="9948a-112">0</span></span>|<span data-ttu-id="9948a-113">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="9948a-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="9948a-114">Пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="9948a-114">pendingInstallation</span></span>|<span data-ttu-id="9948a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="9948a-115">1</span></span>|<span data-ttu-id="9948a-116">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="9948a-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="9948a-117">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="9948a-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="9948a-118">Пендингребут</span><span class="sxs-lookup"><span data-stu-id="9948a-118">pendingReboot</span></span>|<span data-ttu-id="9948a-119">2</span><span class="sxs-lookup"><span data-stu-id="9948a-119">2</span></span>|<span data-ttu-id="9948a-120">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="9948a-120">There are updates that requires reboot.</span></span> <span data-ttu-id="9948a-121">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="9948a-121">There are not failed updates.</span></span>|
|<span data-ttu-id="9948a-122">failed</span><span class="sxs-lookup"><span data-stu-id="9948a-122">failed</span></span>|<span data-ttu-id="9948a-123">4</span><span class="sxs-lookup"><span data-stu-id="9948a-123">3</span></span>|<span data-ttu-id="9948a-124">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9948a-124">There are updates failed to install on the device.</span></span>|




