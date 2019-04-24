---
title: тип перечисления Манажедаппклипбоардшаринглевел
description: Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcbee5e0b7aa6343e31d57d14557bc0f0586fb80
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465204"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="1ca59-103">тип перечисления Манажедаппклипбоардшаринглевел</span><span class="sxs-lookup"><span data-stu-id="1ca59-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="1ca59-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ca59-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ca59-105">Представляет уровень, к которому может быть предоставлен общий доступ к буферу обмена устройства между приложениями</span><span class="sxs-lookup"><span data-stu-id="1ca59-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="1ca59-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="1ca59-106">Members</span></span>
|<span data-ttu-id="1ca59-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="1ca59-107">Member</span></span>|<span data-ttu-id="1ca59-108">Значение</span><span class="sxs-lookup"><span data-stu-id="1ca59-108">Value</span></span>|<span data-ttu-id="1ca59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1ca59-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ca59-110">Аллаппс</span><span class="sxs-lookup"><span data-stu-id="1ca59-110">allApps</span></span>|<span data-ttu-id="1ca59-111">нуль</span><span class="sxs-lookup"><span data-stu-id="1ca59-111">0</span></span>|<span data-ttu-id="1ca59-112">Общий доступ разрешен между всеми приложениями, управляемым или не</span><span class="sxs-lookup"><span data-stu-id="1ca59-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="1ca59-113">Манажедаппсвиспастеин</span><span class="sxs-lookup"><span data-stu-id="1ca59-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="1ca59-114">1,1</span><span class="sxs-lookup"><span data-stu-id="1ca59-114">1</span></span>|<span data-ttu-id="1ca59-115">Разрешен общий доступ для всех управляемых приложений с включенной вставкой</span><span class="sxs-lookup"><span data-stu-id="1ca59-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="1ca59-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="1ca59-116">managedApps</span></span>|<span data-ttu-id="1ca59-117">2</span><span class="sxs-lookup"><span data-stu-id="1ca59-117">2</span></span>|<span data-ttu-id="1ca59-118">Общий доступ разрешен для всех управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="1ca59-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="1ca59-119">заблокированных</span><span class="sxs-lookup"><span data-stu-id="1ca59-119">blocked</span></span>|<span data-ttu-id="1ca59-120">4</span><span class="sxs-lookup"><span data-stu-id="1ca59-120">3</span></span>|<span data-ttu-id="1ca59-121">Совместное использование приложений отключено</span><span class="sxs-lookup"><span data-stu-id="1ca59-121">Sharing between apps is disabled</span></span>|



