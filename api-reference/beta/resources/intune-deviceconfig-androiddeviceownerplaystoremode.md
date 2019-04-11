---
title: тип перечисления Андроиддевицеовнерплайсторемоде
description: Тип режима хранения "владелец устройства Android".
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00909f739773e67d4b5a1ae87f53982b627f511e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809326"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="57815-103">тип перечисления Андроиддевицеовнерплайсторемоде</span><span class="sxs-lookup"><span data-stu-id="57815-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="57815-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57815-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57815-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57815-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57815-106">Тип режима хранения "владелец устройства Android".</span><span class="sxs-lookup"><span data-stu-id="57815-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="57815-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="57815-107">Members</span></span>
|<span data-ttu-id="57815-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="57815-108">Member</span></span>|<span data-ttu-id="57815-109">Значение</span><span class="sxs-lookup"><span data-stu-id="57815-109">Value</span></span>|<span data-ttu-id="57815-110">Описание</span><span class="sxs-lookup"><span data-stu-id="57815-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57815-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="57815-111">notConfigured</span></span>|<span data-ttu-id="57815-112">нуль</span><span class="sxs-lookup"><span data-stu-id="57815-112">0</span></span>|<span data-ttu-id="57815-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="57815-113">Not Configured</span></span>|
|<span data-ttu-id="57815-114">Алловлист</span><span class="sxs-lookup"><span data-stu-id="57815-114">allowList</span></span>|<span data-ttu-id="57815-115">1,1</span><span class="sxs-lookup"><span data-stu-id="57815-115">1</span></span>|<span data-ttu-id="57815-116">С устройства будут автоматически удалены только приложения, наявляющиеся в политике, а все приложения, не включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="57815-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="57815-117">Блокклист</span><span class="sxs-lookup"><span data-stu-id="57815-117">blockList</span></span>|<span data-ttu-id="57815-118">2</span><span class="sxs-lookup"><span data-stu-id="57815-118">2</span></span>|<span data-ttu-id="57815-119">Все приложения доступны, и любое приложение, которое не должно находиться на устройстве, должно быть явно отмечено как ЗАБЛОКИРОВАНо в политике приложений.</span><span class="sxs-lookup"><span data-stu-id="57815-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|





