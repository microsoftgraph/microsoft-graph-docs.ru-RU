---
title: тип перечисления Андроиддевицеовнерплайсторемоде
description: Тип режима хранения "владелец устройства Android".
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 32eb96d5429380eaa6d9f4ffe021d37c62f3fffa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486481"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="0bef0-103">тип перечисления Андроиддевицеовнерплайсторемоде</span><span class="sxs-lookup"><span data-stu-id="0bef0-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

<span data-ttu-id="0bef0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0bef0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bef0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bef0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bef0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bef0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bef0-107">Тип режима хранения "владелец устройства Android".</span><span class="sxs-lookup"><span data-stu-id="0bef0-107">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="0bef0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0bef0-108">Members</span></span>
|<span data-ttu-id="0bef0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0bef0-109">Member</span></span>|<span data-ttu-id="0bef0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0bef0-110">Value</span></span>|<span data-ttu-id="0bef0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0bef0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bef0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0bef0-112">notConfigured</span></span>|<span data-ttu-id="0bef0-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0bef0-113">0</span></span>|<span data-ttu-id="0bef0-114">Not Configured</span><span class="sxs-lookup"><span data-stu-id="0bef0-114">Not Configured</span></span>|
|<span data-ttu-id="0bef0-115">алловлист</span><span class="sxs-lookup"><span data-stu-id="0bef0-115">allowList</span></span>|<span data-ttu-id="0bef0-116">1 </span><span class="sxs-lookup"><span data-stu-id="0bef0-116">1</span></span>|<span data-ttu-id="0bef0-117">С устройства будут автоматически удалены только приложения, наявляющиеся в политике, а все приложения, не включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="0bef0-117">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="0bef0-118">блокклист</span><span class="sxs-lookup"><span data-stu-id="0bef0-118">blockList</span></span>|<span data-ttu-id="0bef0-119">2 </span><span class="sxs-lookup"><span data-stu-id="0bef0-119">2</span></span>|<span data-ttu-id="0bef0-120">Все приложения доступны, и любое приложение, которое не должно находиться на устройстве, должно быть явно отмечено как ЗАБЛОКИРОВАНо в политике приложений.</span><span class="sxs-lookup"><span data-stu-id="0bef0-120">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



