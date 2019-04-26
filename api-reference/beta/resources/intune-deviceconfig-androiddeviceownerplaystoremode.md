---
title: тип перечисления Андроиддевицеовнерплайсторемоде
description: Тип режима хранения "владелец устройства Android".
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00909f739773e67d4b5a1ae87f53982b627f511e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556398"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="0c63a-103">тип перечисления Андроиддевицеовнерплайсторемоде</span><span class="sxs-lookup"><span data-stu-id="0c63a-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="0c63a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c63a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c63a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c63a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c63a-106">Тип режима хранения "владелец устройства Android".</span><span class="sxs-lookup"><span data-stu-id="0c63a-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="0c63a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="0c63a-107">Members</span></span>
|<span data-ttu-id="0c63a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="0c63a-108">Member</span></span>|<span data-ttu-id="0c63a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="0c63a-109">Value</span></span>|<span data-ttu-id="0c63a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0c63a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c63a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0c63a-111">notConfigured</span></span>|<span data-ttu-id="0c63a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="0c63a-112">0</span></span>|<span data-ttu-id="0c63a-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="0c63a-113">Not Configured</span></span>|
|<span data-ttu-id="0c63a-114">Алловлист</span><span class="sxs-lookup"><span data-stu-id="0c63a-114">allowList</span></span>|<span data-ttu-id="0c63a-115">1 </span><span class="sxs-lookup"><span data-stu-id="0c63a-115">1</span></span>|<span data-ttu-id="0c63a-116">С устройства будут автоматически удалены только приложения, наявляющиеся в политике, а все приложения, не включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="0c63a-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="0c63a-117">Блокклист</span><span class="sxs-lookup"><span data-stu-id="0c63a-117">blockList</span></span>|<span data-ttu-id="0c63a-118">2 </span><span class="sxs-lookup"><span data-stu-id="0c63a-118">2</span></span>|<span data-ttu-id="0c63a-119">Все приложения доступны, и любое приложение, которое не должно находиться на устройстве, должно быть явно отмечено как ЗАБЛОКИРОВАНо в политике приложений.</span><span class="sxs-lookup"><span data-stu-id="0c63a-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|





