---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80e2546939b9053eca16607d069689e0226380d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943706"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="b6571-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="b6571-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="b6571-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6571-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6571-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6571-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6571-106">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="b6571-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="b6571-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="b6571-107">Members</span></span>
|<span data-ttu-id="b6571-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="b6571-108">Member</span></span>|<span data-ttu-id="b6571-109">Значение</span><span class="sxs-lookup"><span data-stu-id="b6571-109">Value</span></span>|<span data-ttu-id="b6571-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b6571-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6571-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b6571-111">notConfigured</span></span>|<span data-ttu-id="b6571-112">нуль</span><span class="sxs-lookup"><span data-stu-id="b6571-112">0</span></span>|<span data-ttu-id="b6571-113">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="b6571-113">No access level specified, no intents.</span></span> <span data-ttu-id="b6571-114">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="b6571-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="b6571-115">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="b6571-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="b6571-116">Форцеаллов</span><span class="sxs-lookup"><span data-stu-id="b6571-116">forceAllow</span></span>|<span data-ttu-id="b6571-117">1,1</span><span class="sxs-lookup"><span data-stu-id="b6571-117">1</span></span>|<span data-ttu-id="b6571-118">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b6571-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="b6571-119">Форцедени</span><span class="sxs-lookup"><span data-stu-id="b6571-119">forceDeny</span></span>|<span data-ttu-id="b6571-120">2</span><span class="sxs-lookup"><span data-stu-id="b6571-120">2</span></span>|<span data-ttu-id="b6571-121">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b6571-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="b6571-122">Усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="b6571-122">userInControl</span></span>|<span data-ttu-id="b6571-123">4</span><span class="sxs-lookup"><span data-stu-id="b6571-123">3</span></span>|<span data-ttu-id="b6571-124">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b6571-124">Users will be prompted when apps try to access specified privacy data.</span></span>|




