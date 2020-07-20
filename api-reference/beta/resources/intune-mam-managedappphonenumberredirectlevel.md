---
title: тип перечисления Манажедаппфоненумберредиректлевел
description: Классы приложений, которым разрешено нажатие и открытие номера телефона, для совершения телефонных звонков или отправки текстовых сообщений.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6a291e7d9afc91aa93b3cfe5d5636383fcf2ace6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793873"
---
# <a name="managedappphonenumberredirectlevel-enum-type"></a><span data-ttu-id="bd466-103">тип перечисления Манажедаппфоненумберредиректлевел</span><span class="sxs-lookup"><span data-stu-id="bd466-103">managedAppPhoneNumberRedirectLevel enum type</span></span>

<span data-ttu-id="bd466-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd466-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd466-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd466-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd466-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd466-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd466-107">Классы приложений, которым разрешено нажатие и открытие номера телефона, для совершения телефонных звонков или отправки текстовых сообщений.</span><span class="sxs-lookup"><span data-stu-id="bd466-107">The classes of apps that are allowed to click-to-open a phone number, for making phone calls or sending text messages.</span></span>

## <a name="members"></a><span data-ttu-id="bd466-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="bd466-108">Members</span></span>
|<span data-ttu-id="bd466-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="bd466-109">Member</span></span>|<span data-ttu-id="bd466-110">Значение</span><span class="sxs-lookup"><span data-stu-id="bd466-110">Value</span></span>|<span data-ttu-id="bd466-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd466-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd466-112">аллаппс</span><span class="sxs-lookup"><span data-stu-id="bd466-112">allApps</span></span>|<span data-ttu-id="bd466-113">нуль</span><span class="sxs-lookup"><span data-stu-id="bd466-113">0</span></span>|<span data-ttu-id="bd466-114">Предоставление общего доступа разрешено для всех приложений.</span><span class="sxs-lookup"><span data-stu-id="bd466-114">Sharing is allowed to all apps.</span></span>|
|<span data-ttu-id="bd466-115">managedApps</span><span class="sxs-lookup"><span data-stu-id="bd466-115">managedApps</span></span>|<span data-ttu-id="bd466-116">1 </span><span class="sxs-lookup"><span data-stu-id="bd466-116">1</span></span>|<span data-ttu-id="bd466-117">Общий доступ разрешен всем управляемым приложениям.</span><span class="sxs-lookup"><span data-stu-id="bd466-117">Sharing is allowed to all managed apps.</span></span>|
|<span data-ttu-id="bd466-118">customApp</span><span class="sxs-lookup"><span data-stu-id="bd466-118">customApp</span></span>|<span data-ttu-id="bd466-119">2</span><span class="sxs-lookup"><span data-stu-id="bd466-119">2</span></span>|<span data-ttu-id="bd466-120">Общий доступ разрешен для настраиваемого приложения.</span><span class="sxs-lookup"><span data-stu-id="bd466-120">Sharing is allowed to a custom app.</span></span>|
|<span data-ttu-id="bd466-121">заблокированных</span><span class="sxs-lookup"><span data-stu-id="bd466-121">blocked</span></span>|<span data-ttu-id="bd466-122">4</span><span class="sxs-lookup"><span data-stu-id="bd466-122">3</span></span>|<span data-ttu-id="bd466-123">Совместное использование приложений заблокировано.</span><span class="sxs-lookup"><span data-stu-id="bd466-123">Sharing between apps is blocked.</span></span>|



