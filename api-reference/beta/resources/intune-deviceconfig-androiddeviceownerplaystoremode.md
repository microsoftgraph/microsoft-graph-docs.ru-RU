---
title: тип перечисления Андроиддевицеовнерплайсторемоде
description: Тип режима хранения "владелец устройства Android".
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3f13a942c5b678367262400aeeea9c80ed705b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983808"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="b1d09-103">тип перечисления Андроиддевицеовнерплайсторемоде</span><span class="sxs-lookup"><span data-stu-id="b1d09-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="b1d09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1d09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1d09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1d09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1d09-106">Тип режима хранения "владелец устройства Android".</span><span class="sxs-lookup"><span data-stu-id="b1d09-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="b1d09-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b1d09-107">Members</span></span>
|<span data-ttu-id="b1d09-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b1d09-108">Member</span></span>|<span data-ttu-id="b1d09-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b1d09-109">Value</span></span>|<span data-ttu-id="b1d09-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1d09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1d09-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b1d09-111">notConfigured</span></span>|<span data-ttu-id="b1d09-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b1d09-112">0</span></span>|<span data-ttu-id="b1d09-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="b1d09-113">Not Configured</span></span>|
|<span data-ttu-id="b1d09-114">Алловлист</span><span class="sxs-lookup"><span data-stu-id="b1d09-114">allowList</span></span>|<span data-ttu-id="b1d09-115">1,1</span><span class="sxs-lookup"><span data-stu-id="b1d09-115">1</span></span>|<span data-ttu-id="b1d09-116">С устройства будут автоматически удалены только приложения, наявляющиеся в политике, а все приложения, не включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="b1d09-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="b1d09-117">Блокклист</span><span class="sxs-lookup"><span data-stu-id="b1d09-117">blockList</span></span>|<span data-ttu-id="b1d09-118">2</span><span class="sxs-lookup"><span data-stu-id="b1d09-118">2</span></span>|<span data-ttu-id="b1d09-119">Все приложения доступны, и любое приложение, которое не должно находиться на устройстве, должно быть явно отмечено как ЗАБЛОКИРОВАНо в политике приложений.</span><span class="sxs-lookup"><span data-stu-id="b1d09-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|





