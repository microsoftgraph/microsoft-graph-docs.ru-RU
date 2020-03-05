---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 90fb42248dc0bc78e33c18150b59d88487a6a06b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525371"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="ba059-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="ba059-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="ba059-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ba059-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba059-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba059-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba059-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba059-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba059-107">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="ba059-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="ba059-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ba059-108">Members</span></span>
|<span data-ttu-id="ba059-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ba059-109">Member</span></span>|<span data-ttu-id="ba059-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ba059-110">Value</span></span>|<span data-ttu-id="ba059-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ba059-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba059-112">уптодате</span><span class="sxs-lookup"><span data-stu-id="ba059-112">upToDate</span></span>|<span data-ttu-id="ba059-113">нуль</span><span class="sxs-lookup"><span data-stu-id="ba059-113">0</span></span>|<span data-ttu-id="ba059-114">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="ba059-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="ba059-115">пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="ba059-115">pendingInstallation</span></span>|<span data-ttu-id="ba059-116">1 </span><span class="sxs-lookup"><span data-stu-id="ba059-116">1</span></span>|<span data-ttu-id="ba059-117">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="ba059-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="ba059-118">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="ba059-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="ba059-119">пендингребут</span><span class="sxs-lookup"><span data-stu-id="ba059-119">pendingReboot</span></span>|<span data-ttu-id="ba059-120">2 </span><span class="sxs-lookup"><span data-stu-id="ba059-120">2</span></span>|<span data-ttu-id="ba059-121">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="ba059-121">There are updates that requires reboot.</span></span> <span data-ttu-id="ba059-122">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="ba059-122">There are not failed updates.</span></span>|
|<span data-ttu-id="ba059-123">сбоев</span><span class="sxs-lookup"><span data-stu-id="ba059-123">failed</span></span>|<span data-ttu-id="ba059-124">3 </span><span class="sxs-lookup"><span data-stu-id="ba059-124">3</span></span>|<span data-ttu-id="ba059-125">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ba059-125">There are updates failed to install on the device.</span></span>|



