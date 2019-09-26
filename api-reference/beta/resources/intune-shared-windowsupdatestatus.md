---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ce9ae47680408f50ef5ce42606cd856ac13ddc1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201193"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="2b7a0-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="2b7a0-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="2b7a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b7a0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b7a0-106">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="2b7a0-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="2b7a0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2b7a0-107">Members</span></span>
|<span data-ttu-id="2b7a0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2b7a0-108">Member</span></span>|<span data-ttu-id="2b7a0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2b7a0-109">Value</span></span>|<span data-ttu-id="2b7a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b7a0-111">уптодате</span><span class="sxs-lookup"><span data-stu-id="2b7a0-111">upToDate</span></span>|<span data-ttu-id="2b7a0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2b7a0-112">0</span></span>|<span data-ttu-id="2b7a0-113">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="2b7a0-114">пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="2b7a0-114">pendingInstallation</span></span>|<span data-ttu-id="2b7a0-115">1,1</span><span class="sxs-lookup"><span data-stu-id="2b7a0-115">1</span></span>|<span data-ttu-id="2b7a0-116">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="2b7a0-117">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="2b7a0-118">пендингребут</span><span class="sxs-lookup"><span data-stu-id="2b7a0-118">pendingReboot</span></span>|<span data-ttu-id="2b7a0-119">2</span><span class="sxs-lookup"><span data-stu-id="2b7a0-119">2</span></span>|<span data-ttu-id="2b7a0-120">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-120">There are updates that requires reboot.</span></span> <span data-ttu-id="2b7a0-121">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-121">There are not failed updates.</span></span>|
|<span data-ttu-id="2b7a0-122">сбоев</span><span class="sxs-lookup"><span data-stu-id="2b7a0-122">failed</span></span>|<span data-ttu-id="2b7a0-123">4</span><span class="sxs-lookup"><span data-stu-id="2b7a0-123">3</span></span>|<span data-ttu-id="2b7a0-124">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2b7a0-124">There are updates failed to install on the device.</span></span>|



