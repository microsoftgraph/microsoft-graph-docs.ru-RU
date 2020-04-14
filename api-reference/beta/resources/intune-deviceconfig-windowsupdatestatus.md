---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ac307aae8f43cd423c41c1a20ccbc7b9928452d3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441095"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="81b80-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="81b80-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="81b80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81b80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81b80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81b80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81b80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81b80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81b80-107">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="81b80-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="81b80-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="81b80-108">Members</span></span>
|<span data-ttu-id="81b80-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="81b80-109">Member</span></span>|<span data-ttu-id="81b80-110">Значение</span><span class="sxs-lookup"><span data-stu-id="81b80-110">Value</span></span>|<span data-ttu-id="81b80-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81b80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b80-112">уптодате</span><span class="sxs-lookup"><span data-stu-id="81b80-112">upToDate</span></span>|<span data-ttu-id="81b80-113">нуль</span><span class="sxs-lookup"><span data-stu-id="81b80-113">0</span></span>|<span data-ttu-id="81b80-114">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="81b80-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="81b80-115">пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="81b80-115">pendingInstallation</span></span>|<span data-ttu-id="81b80-116">1,1</span><span class="sxs-lookup"><span data-stu-id="81b80-116">1</span></span>|<span data-ttu-id="81b80-117">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="81b80-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="81b80-118">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="81b80-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="81b80-119">пендингребут</span><span class="sxs-lookup"><span data-stu-id="81b80-119">pendingReboot</span></span>|<span data-ttu-id="81b80-120">2</span><span class="sxs-lookup"><span data-stu-id="81b80-120">2</span></span>|<span data-ttu-id="81b80-121">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="81b80-121">There are updates that requires reboot.</span></span> <span data-ttu-id="81b80-122">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="81b80-122">There are not failed updates.</span></span>|
|<span data-ttu-id="81b80-123">сбоев</span><span class="sxs-lookup"><span data-stu-id="81b80-123">failed</span></span>|<span data-ttu-id="81b80-124">4</span><span class="sxs-lookup"><span data-stu-id="81b80-124">3</span></span>|<span data-ttu-id="81b80-125">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="81b80-125">There are updates failed to install on the device.</span></span>|



