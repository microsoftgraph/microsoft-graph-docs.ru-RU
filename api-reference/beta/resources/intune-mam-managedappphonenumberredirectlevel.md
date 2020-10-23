---
title: тип перечисления Манажедаппфоненумберредиректлевел
description: Классы приложений, которым разрешено нажатие и открытие номера телефона, для совершения телефонных звонков или отправки текстовых сообщений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1b0e37364bd505dada24d0283477742f70183b83
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722811"
---
# <a name="managedappphonenumberredirectlevel-enum-type"></a><span data-ttu-id="c7249-103">тип перечисления Манажедаппфоненумберредиректлевел</span><span class="sxs-lookup"><span data-stu-id="c7249-103">managedAppPhoneNumberRedirectLevel enum type</span></span>

<span data-ttu-id="c7249-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7249-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7249-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7249-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7249-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7249-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7249-107">Классы приложений, которым разрешено нажатие и открытие номера телефона, для совершения телефонных звонков или отправки текстовых сообщений.</span><span class="sxs-lookup"><span data-stu-id="c7249-107">The classes of apps that are allowed to click-to-open a phone number, for making phone calls or sending text messages.</span></span>

## <a name="members"></a><span data-ttu-id="c7249-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c7249-108">Members</span></span>
|<span data-ttu-id="c7249-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c7249-109">Member</span></span>|<span data-ttu-id="c7249-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c7249-110">Value</span></span>|<span data-ttu-id="c7249-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7249-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7249-112">аллаппс</span><span class="sxs-lookup"><span data-stu-id="c7249-112">allApps</span></span>|<span data-ttu-id="c7249-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c7249-113">0</span></span>|<span data-ttu-id="c7249-114">Предоставление общего доступа разрешено для всех приложений.</span><span class="sxs-lookup"><span data-stu-id="c7249-114">Sharing is allowed to all apps.</span></span>|
|<span data-ttu-id="c7249-115">managedApps</span><span class="sxs-lookup"><span data-stu-id="c7249-115">managedApps</span></span>|<span data-ttu-id="c7249-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c7249-116">1</span></span>|<span data-ttu-id="c7249-117">Общий доступ разрешен всем управляемым приложениям.</span><span class="sxs-lookup"><span data-stu-id="c7249-117">Sharing is allowed to all managed apps.</span></span>|
|<span data-ttu-id="c7249-118">customApp</span><span class="sxs-lookup"><span data-stu-id="c7249-118">customApp</span></span>|<span data-ttu-id="c7249-119">2</span><span class="sxs-lookup"><span data-stu-id="c7249-119">2</span></span>|<span data-ttu-id="c7249-120">Общий доступ разрешен для настраиваемого приложения.</span><span class="sxs-lookup"><span data-stu-id="c7249-120">Sharing is allowed to a custom app.</span></span>|
|<span data-ttu-id="c7249-121">заблокированных</span><span class="sxs-lookup"><span data-stu-id="c7249-121">blocked</span></span>|<span data-ttu-id="c7249-122">4</span><span class="sxs-lookup"><span data-stu-id="c7249-122">3</span></span>|<span data-ttu-id="c7249-123">Совместное использование приложений заблокировано.</span><span class="sxs-lookup"><span data-stu-id="c7249-123">Sharing between apps is blocked.</span></span>|





