---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0151a572011f9033ae7b622e5d3cf2bfd086ed39
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706935"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="9d616-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="9d616-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="9d616-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d616-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d616-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d616-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d616-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d616-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d616-107">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="9d616-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="9d616-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9d616-108">Members</span></span>
|<span data-ttu-id="9d616-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9d616-109">Member</span></span>|<span data-ttu-id="9d616-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9d616-110">Value</span></span>|<span data-ttu-id="9d616-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9d616-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d616-112">уптодате</span><span class="sxs-lookup"><span data-stu-id="9d616-112">upToDate</span></span>|<span data-ttu-id="9d616-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9d616-113">0</span></span>|<span data-ttu-id="9d616-114">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="9d616-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="9d616-115">пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="9d616-115">pendingInstallation</span></span>|<span data-ttu-id="9d616-116">1,1</span><span class="sxs-lookup"><span data-stu-id="9d616-116">1</span></span>|<span data-ttu-id="9d616-117">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="9d616-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="9d616-118">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="9d616-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="9d616-119">пендингребут</span><span class="sxs-lookup"><span data-stu-id="9d616-119">pendingReboot</span></span>|<span data-ttu-id="9d616-120">2</span><span class="sxs-lookup"><span data-stu-id="9d616-120">2</span></span>|<span data-ttu-id="9d616-121">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="9d616-121">There are updates that requires reboot.</span></span> <span data-ttu-id="9d616-122">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="9d616-122">There are not failed updates.</span></span>|
|<span data-ttu-id="9d616-123">сбоев</span><span class="sxs-lookup"><span data-stu-id="9d616-123">failed</span></span>|<span data-ttu-id="9d616-124">4</span><span class="sxs-lookup"><span data-stu-id="9d616-124">3</span></span>|<span data-ttu-id="9d616-125">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9d616-125">There are updates failed to install on the device.</span></span>|





