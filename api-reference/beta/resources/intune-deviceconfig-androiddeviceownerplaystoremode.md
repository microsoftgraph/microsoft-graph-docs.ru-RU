---
title: тип перечисления Андроиддевицеовнерплайсторемоде
description: Тип режима хранения "владелец устройства Android".
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d883091a7162c7cb0da40113430edbdc66a9cfa7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334810"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="bb52e-103">тип перечисления Андроиддевицеовнерплайсторемоде</span><span class="sxs-lookup"><span data-stu-id="bb52e-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="bb52e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb52e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb52e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb52e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb52e-106">Тип режима хранения "владелец устройства Android".</span><span class="sxs-lookup"><span data-stu-id="bb52e-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="bb52e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="bb52e-107">Members</span></span>
|<span data-ttu-id="bb52e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="bb52e-108">Member</span></span>|<span data-ttu-id="bb52e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="bb52e-109">Value</span></span>|<span data-ttu-id="bb52e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb52e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb52e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bb52e-111">notConfigured</span></span>|<span data-ttu-id="bb52e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="bb52e-112">0</span></span>|<span data-ttu-id="bb52e-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="bb52e-113">Not Configured</span></span>|
|<span data-ttu-id="bb52e-114">алловлист</span><span class="sxs-lookup"><span data-stu-id="bb52e-114">allowList</span></span>|<span data-ttu-id="bb52e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="bb52e-115">1</span></span>|<span data-ttu-id="bb52e-116">С устройства будут автоматически удалены только приложения, наявляющиеся в политике, а все приложения, не включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="bb52e-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="bb52e-117">блокклист</span><span class="sxs-lookup"><span data-stu-id="bb52e-117">blockList</span></span>|<span data-ttu-id="bb52e-118">2</span><span class="sxs-lookup"><span data-stu-id="bb52e-118">2</span></span>|<span data-ttu-id="bb52e-119">Все приложения доступны, и любое приложение, которое не должно находиться на устройстве, должно быть явно отмечено как ЗАБЛОКИРОВАНо в политике приложений.</span><span class="sxs-lookup"><span data-stu-id="bb52e-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



