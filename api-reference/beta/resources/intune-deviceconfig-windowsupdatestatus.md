---
title: тип перечисления Виндовсупдатестатус
description: Состояния устройств конфигурации центра обновления Windows для бизнеса
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a09aca9ce1ac4cd81e09b8db8da10ea563f1f03
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272369"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="b2aad-103">тип перечисления Виндовсупдатестатус</span><span class="sxs-lookup"><span data-stu-id="b2aad-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="b2aad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2aad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2aad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2aad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2aad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2aad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2aad-107">Состояния устройств конфигурации центра обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b2aad-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="b2aad-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b2aad-108">Members</span></span>
|<span data-ttu-id="b2aad-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b2aad-109">Member</span></span>|<span data-ttu-id="b2aad-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b2aad-110">Value</span></span>|<span data-ttu-id="b2aad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2aad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2aad-112">уптодате</span><span class="sxs-lookup"><span data-stu-id="b2aad-112">upToDate</span></span>|<span data-ttu-id="b2aad-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b2aad-113">0</span></span>|<span data-ttu-id="b2aad-114">Нет ожидающих обновлений, ожидающих обновлений для перезагрузки и без сбоев обновлений.</span><span class="sxs-lookup"><span data-stu-id="b2aad-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="b2aad-115">пендингинсталлатион</span><span class="sxs-lookup"><span data-stu-id="b2aad-115">pendingInstallation</span></span>|<span data-ttu-id="b2aad-116">1,1</span><span class="sxs-lookup"><span data-stu-id="b2aad-116">1</span></span>|<span data-ttu-id="b2aad-117">Существуют обновления, ожидающие установки, которые включают Неутвержденные обновления.</span><span class="sxs-lookup"><span data-stu-id="b2aad-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="b2aad-118">Нет обновлений, ожидающих перезагрузки, неудачных обновлений.</span><span class="sxs-lookup"><span data-stu-id="b2aad-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="b2aad-119">пендингребут</span><span class="sxs-lookup"><span data-stu-id="b2aad-119">pendingReboot</span></span>|<span data-ttu-id="b2aad-120">2</span><span class="sxs-lookup"><span data-stu-id="b2aad-120">2</span></span>|<span data-ttu-id="b2aad-121">Существуют обновления, требующие перезагрузки.</span><span class="sxs-lookup"><span data-stu-id="b2aad-121">There are updates that requires reboot.</span></span> <span data-ttu-id="b2aad-122">Обновления не выполнены.</span><span class="sxs-lookup"><span data-stu-id="b2aad-122">There are not failed updates.</span></span>|
|<span data-ttu-id="b2aad-123">сбоев</span><span class="sxs-lookup"><span data-stu-id="b2aad-123">failed</span></span>|<span data-ttu-id="b2aad-124">4</span><span class="sxs-lookup"><span data-stu-id="b2aad-124">3</span></span>|<span data-ttu-id="b2aad-125">Не удалось установить обновления на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b2aad-125">There are updates failed to install on the device.</span></span>|




