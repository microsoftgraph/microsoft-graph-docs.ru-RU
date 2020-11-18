---
title: тип перечисления Андроиддевицеовнерплайсторемоде
description: Тип режима хранения "владелец устройства Android".
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 899f3fab4bd0e6172b7fd16182d8195c427deb23
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199961"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="e2e29-103">тип перечисления Андроиддевицеовнерплайсторемоде</span><span class="sxs-lookup"><span data-stu-id="e2e29-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

<span data-ttu-id="e2e29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2e29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2e29-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2e29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2e29-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2e29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2e29-107">Тип режима хранения "владелец устройства Android".</span><span class="sxs-lookup"><span data-stu-id="e2e29-107">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="e2e29-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e2e29-108">Members</span></span>
|<span data-ttu-id="e2e29-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e2e29-109">Member</span></span>|<span data-ttu-id="e2e29-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e2e29-110">Value</span></span>|<span data-ttu-id="e2e29-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e2e29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e29-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e2e29-112">notConfigured</span></span>|<span data-ttu-id="e2e29-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e2e29-113">0</span></span>|<span data-ttu-id="e2e29-114">Not Configured</span><span class="sxs-lookup"><span data-stu-id="e2e29-114">Not Configured</span></span>|
|<span data-ttu-id="e2e29-115">алловлист</span><span class="sxs-lookup"><span data-stu-id="e2e29-115">allowList</span></span>|<span data-ttu-id="e2e29-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e2e29-116">1</span></span>|<span data-ttu-id="e2e29-117">С устройства будут автоматически удалены только приложения, наявляющиеся в политике, а все приложения, не включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="e2e29-117">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="e2e29-118">блокклист</span><span class="sxs-lookup"><span data-stu-id="e2e29-118">blockList</span></span>|<span data-ttu-id="e2e29-119">2</span><span class="sxs-lookup"><span data-stu-id="e2e29-119">2</span></span>|<span data-ttu-id="e2e29-120">Все приложения доступны, и любое приложение, которое не должно находиться на устройстве, должно быть явно отмечено как ЗАБЛОКИРОВАНо в политике приложений.</span><span class="sxs-lookup"><span data-stu-id="e2e29-120">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|




