---
title: тип перечисления Иоснотификатионпревиеввисибилити
description: Определяет, отображаются ли эскизы уведомлений на устройстве с iOS. Предварительный просмотр может включать такие сведения, как текст (из сообщений и почта), а также сведения о приглашении (из календаря). При настройке это приведет к переопределению пользовательских параметров предварительного просмотра.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 607e771ce83858cd22892efa9a377b7997142a24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302226"
---
# <a name="iosnotificationpreviewvisibility-enum-type"></a><span data-ttu-id="b2c90-105">тип перечисления Иоснотификатионпревиеввисибилити</span><span class="sxs-lookup"><span data-stu-id="b2c90-105">iosNotificationPreviewVisibility enum type</span></span>

<span data-ttu-id="b2c90-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2c90-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2c90-107">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2c90-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2c90-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2c90-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2c90-109">Определяет, отображаются ли эскизы уведомлений на устройстве с iOS.</span><span class="sxs-lookup"><span data-stu-id="b2c90-109">Determines when notification previews are visible on an iOS device.</span></span> <span data-ttu-id="b2c90-110">Предварительный просмотр может включать такие сведения, как текст (из сообщений и почта), а также сведения о приглашении (из календаря).</span><span class="sxs-lookup"><span data-stu-id="b2c90-110">Previews can include things like text (from Messages and Mail) and invitation details (from Calendar).</span></span> <span data-ttu-id="b2c90-111">При настройке это приведет к переопределению пользовательских параметров предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="b2c90-111">When configured, it will override the user's defined preview settings.</span></span>

## <a name="members"></a><span data-ttu-id="b2c90-112">Элементы</span><span class="sxs-lookup"><span data-stu-id="b2c90-112">Members</span></span>
|<span data-ttu-id="b2c90-113">Элемент</span><span class="sxs-lookup"><span data-stu-id="b2c90-113">Member</span></span>|<span data-ttu-id="b2c90-114">Значение</span><span class="sxs-lookup"><span data-stu-id="b2c90-114">Value</span></span>|<span data-ttu-id="b2c90-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b2c90-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c90-116">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b2c90-116">notConfigured</span></span>|<span data-ttu-id="b2c90-117">нуль</span><span class="sxs-lookup"><span data-stu-id="b2c90-117">0</span></span>|<span data-ttu-id="b2c90-118">Параметры предварительного просмотра уведомлений не будут перезаписаны.</span><span class="sxs-lookup"><span data-stu-id="b2c90-118">Notification preview settings will not be overwritten.</span></span>|
|<span data-ttu-id="b2c90-119">алвайсшов</span><span class="sxs-lookup"><span data-stu-id="b2c90-119">alwaysShow</span></span>|<span data-ttu-id="b2c90-120">1,1</span><span class="sxs-lookup"><span data-stu-id="b2c90-120">1</span></span>|<span data-ttu-id="b2c90-121">Всегда показывать предварительные Просмотр уведомлений.</span><span class="sxs-lookup"><span data-stu-id="b2c90-121">Always show notification previews.</span></span>|
|<span data-ttu-id="b2c90-122">хидевхенлоккед</span><span class="sxs-lookup"><span data-stu-id="b2c90-122">hideWhenLocked</span></span>|<span data-ttu-id="b2c90-123">2</span><span class="sxs-lookup"><span data-stu-id="b2c90-123">2</span></span>|<span data-ttu-id="b2c90-124">Показывать только предварительный просмотр уведомлений, только когда устройство разблокировано.</span><span class="sxs-lookup"><span data-stu-id="b2c90-124">Only show notification previews when the device is unlocked.</span></span>|
|<span data-ttu-id="b2c90-125">невершов</span><span class="sxs-lookup"><span data-stu-id="b2c90-125">neverShow</span></span>|<span data-ttu-id="b2c90-126">4</span><span class="sxs-lookup"><span data-stu-id="b2c90-126">3</span></span>|<span data-ttu-id="b2c90-127">Никогда не показывать предварительные Просмотр уведомлений.</span><span class="sxs-lookup"><span data-stu-id="b2c90-127">Never show notification previews.</span></span>|




